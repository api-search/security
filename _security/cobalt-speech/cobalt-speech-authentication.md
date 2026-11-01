---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cobalt-speech-openapi-generated.yml
  format: yaml
  label: Cobalt Speech API
  slug: cobalt-speech-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cobalt-speech/openapi/_ae-authored/cobalt-speech-openapi-generated.yml
auth_types: []
description: Client authentication is performed via mutually authenticated TLS (mTLS). The client must present a PEM‑encoded certificate and private key (and optionally a root certificate) when establishing the gRPC TLS connection.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Cobalt Speech Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cobalt Speech declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Cobalt Speech
provider_slug: cobalt-speech
scheme_count: 1
schemes:
- evidence: If your Transcribe server is configured to do client authentication, you will need to present the appropriate certificate and key when connecting to it.
  how_to_obtain: Obtain a client certificate and private key from the server administrator and provide them to the gRPC client library (e.g., via grpc.ssl_channel_credentials with root_certificates, private_key, and certificate_chain).
  location: TLS handshake (certificate and key supplied to grpc.ssl_channel_credentials or credentials.NewTLS)
  name: mutual TLS
  type: mtls
slug: cobalt-speech-authentication
source_filename: cobalt-speech-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.cobaltspeech.com/docs/asr/transcribe/client_quickstart/
source_yaml: "generated: '2026-10-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.cobaltspeech.com/docs/asr/transcribe/client_quickstart/\nsources:\n- https://docs.cobaltspeech.com/docs/asr/transcribe/client_quickstart/\n- https://docs.cobaltspeech.com/docs/asr/transcribe/setup_connection/\n- https://docs.cobaltspeech.com/docs/speech_assessment/capt/setup_connection/\n- https://docs.cobaltspeech.com/docs/voice_intelligence/voicebio/setup_connection/\ndescription: Client authentication is performed via mutually authenticated TLS (mTLS). The client must present a PEM‑encoded certificate and private\n  key (and optionally a root certificate) when establishing the gRPC TLS connection.\nschemes:\n- type: mtls\n  name: mutual TLS\n  evidence: If your Transcribe server is configured to do client authentication, you will need to present the appropriate certificate and key\n    when connecting to it.\n  location: TLS handshake (certificate and key supplied\
  \ to grpc.ssl_channel_credentials or credentials.NewTLS)\n  how_to_obtain: Obtain a client certificate and private key from the server administrator and provide them to the gRPC client library (e.g.,\n    via grpc.ssl_channel_credentials with root_certificates, private_key, and certificate_chain).\nnote: No other authentication mechanisms (apiKey, oauth2, http‑bearer, etc.) are documented on the provided pages.\ndocs: https://docs.cobaltspeech.com/docs/asr/transcribe/client_quickstart/\n"
source_yaml_url: https://artifacts.apis.io/cobalt-speech/authentication/cobalt-speech-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Speech
- AI
- Transcription
- Voice
---
