# cadence-apis
ConnectRPC API Protobuf Files for Cadence APIs

**WARNING: This API is currently designed for internal use and is entirely unstable. 'v1' is the wrong naming scheme for this type of release. Please expect breaking changes until further notice.**

## Available APIs
- Cadence Users
- Cadence Scorify
- Cadence HCM and HRIS (via hr and shifts packages)

## TODO's
- Inline with best practices, include some form of version field. [Link](https://protobuf.dev/programming-guides/api/#include-version-field)

## Notes:
- All requests **must** specify a field mask. This is to ensure that the client is aware of the fields that are being returned. This is to prevent unnecessary data transfer and to ensure that the client is aware of the fields that are being returned. [Link](https://protobuf.dev/reference/protobuf/google.protobuf/#field-mask)
- Wildcard field masks are not supported. You must explicitly specify the fields that you want to return.