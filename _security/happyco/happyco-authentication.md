---
api_key_in:
- metadata
auth_types:
- http-basic
description: ''
kind: authentication
layout: security
method: searched
name: Happyco Authentication
name_suffix: Authentication
oauth_flows: []
overview: HappyCo secures its APIs with http-basic across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HappyCo
provider_slug: happyco
scheme_count: 1
schemes:
- credentials:
    client_id: HAPPYCO_CLIENT_ID
    client_secret: HAPPYCO_CLIENT_SECRET
  description: HTTP Basic authentication carried as gRPC call credentials. The client encodes "<client_id>:<client_secret>" with Base64 and sends it in the gRPC `authorization` metadata header ("Basic <base64>"). Call credentials are composed onto channel (TLS) credentials, so all traffic is encrypted in transit to grpc.happyco.com.
  name: BasicAuth
  scheme: basic
  sources:
  - github.com/happy-co/api-ruby (examples/auth/auth.rb)
  type: http
slug: happyco-authentication
source_filename: happyco-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://github.com/happy-co/api-ruby/blob/master/examples/auth/auth.rb\ndocs: https://developer.happy.co/downloads/overview.pdf\nsummary:\n  transport: grpc\n  types: [http-basic]\n  api_key_in: [metadata]\n  oauth2_flows: []\nhost: grpc.happyco.com\nschemes:\n  - name: BasicAuth\n    type: http\n    scheme: basic\n    description: >-\n      HTTP Basic authentication carried as gRPC call credentials. The client\n      encodes \"<client_id>:<client_secret>\" with Base64 and sends it in the\n      gRPC `authorization` metadata header (\"Basic <base64>\"). Call credentials\n      are composed onto channel (TLS) credentials, so all traffic is encrypted\n      in transit to grpc.happyco.com.\n    credentials:\n      client_id: HAPPYCO_CLIENT_ID\n      client_secret: HAPPYCO_CLIENT_SECRET\n    sources:\n      - github.com/happy-co/api-ruby (examples/auth/auth.rb)\nnotes: >-\n  HappyCo issues per-integration client_id / client_secret\
  \ credentials. There is\n  no OAuth2/OIDC surface and no API-key query parameter — auth is Basic over the\n  gRPC channel. Partner integrations that provision sub-accounts use the same\n  credential scoped to the AccountProvisioning service.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/happyco/refs/heads/main/authentication/happyco-authentication.yml
summary_line: http-basic · 1 scheme
tags:
- Company
- PropTech
- Real Estate
- Property Management
- Inspections
- Maintenance
- Multifamily
- gRPC
---
