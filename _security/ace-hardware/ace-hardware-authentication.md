---
api_key_in: []
auth_types: []
description: Authentication profile for Ace Hardware's integration surfaces. There is no OpenAPI securitySchemes block to derive from — Ace Hardware publishes no HTTP API — so this profile is searched from the provider's vendor documentation and affiliate program pages. The controlling credential on the machine-to-machine surface is an X.509 certificate used for AS2 message signing and encryption, not an API key or a bearer token.
kind: authentication
layout: security
method: searched
name: Ace Hardware Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ace Hardware declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Ace Hardware
provider_slug: ace-hardware
scheme_count: 3
schemes:
- credential: X.509 certificate pair exchanged during trading-partner setup
  description: Vendors exchange X12 documents with Ace Hardware over AS2 (HTTP or HTTPS). Authentication and encryption are provided by exchanged X.509 certificates; Ace states a preference for SHA2. Certificates are swapped during trading-partner setup along with the AS2 identifiers, so credential issuance is a manual onboarding step, not a self-service key.
  evidence: '"Ace Hardware offers data exchange over the internet using AS2 HTTP or HTTP/HTTPS with authentication and encryption provided via certificate (preferred being SHA2)."'
  id: as2-certificate
  identifiers:
  - edi_id: ZZ/7089906600
    environment: stage
  - edi_id: 01/006928311
    environment: production
  self_service: false
  signature_algorithm_preference: SHA2
  subtype: as2-message-level-certificate
  surface: Ace Hardware Vendor EDI Integration
  type: mutualTLS
- description: The vendor portal at www.acehardware-vendors.com serves a public documents area (the Ace Vendor Manual and forms are readable anonymously) behind which vendor-specific functions require a portal account issued by Ace Hardware. No public registration path exists.
  evidence: https://www.acehardware-vendors.com/ returned 200 with a public Vendors Public documents area and a login for vendor-specific functions (probed 2026-08-30).
  id: vendor-portal-login
  self_service: false
  subtype: session-login
  surface: AceHardware-Vendors.com vendor portal
  type: http
- description: The affiliate program is operated on the Impact partner network. Tracking links, banners and reporting are accessed with an Impact media-partner account, not with an Ace Hardware credential. Any programmatic access to affiliate reporting is Impact's API under Impact's own credentials — Ace Hardware issues no affiliate API key.
  evidence: https://www.acehardware.com/affiliates states "You can find reporting, links, and banners at Impact!" and links the media-partner signup.
  id: impact-affiliate-account
  self_service: true
  signup: https://app.impact.com/campaign-mediapartner-signup/Ace-Hardware.brand?type=dm
  subtype: third-party-network-account
  surface: Ace Hardware Affiliate Program
  type: delegated
slug: ace-hardware-authentication
source_filename: ace-hardware-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: searched\nsource: >-\n  https://www.acehardware-vendors.com/Vendors%20Public/Documents/Ace%20Vendor%20Manual.pdf\n  and https://www.acehardware.com/affiliates\ndocs: https://www.acehardware-vendors.com/\nprovider: Ace Hardware\nproviderId: ace-hardware\ndescription: >-\n  Authentication profile for Ace Hardware's integration surfaces. There is no OpenAPI\n  securitySchemes block to derive from — Ace Hardware publishes no HTTP API — so this profile is\n  searched from the provider's vendor documentation and affiliate program pages. The controlling\n  credential on the machine-to-machine surface is an X.509 certificate used for AS2 message\n  signing and encryption, not an API key or a bearer token.\nnote: >-\n  derive-authentication.py was not applicable here: it reads openapi/ and this repo has no\n  OpenAPI document because the provider publishes none.\n\nschemes:\n  - id: as2-certificate\n    type: mutualTLS\n    subtype: as2-message-level-certificate\n\
  \    surface: Ace Hardware Vendor EDI Integration\n    description: >-\n      Vendors exchange X12 documents with Ace Hardware over AS2 (HTTP or HTTPS). Authentication\n      and encryption are provided by exchanged X.509 certificates; Ace states a preference for\n      SHA2. Certificates are swapped during trading-partner setup along with the AS2 identifiers,\n      so credential issuance is a manual onboarding step, not a self-service key.\n    credential: X.509 certificate pair exchanged during trading-partner setup\n    signature_algorithm_preference: SHA2\n    identifiers:\n      - environment: stage\n        edi_id: ZZ/7089906600\n      - environment: production\n        edi_id: 01/006928311\n    self_service: false\n    evidence: >-\n      \"Ace Hardware offers data exchange over the internet using AS2 HTTP or HTTP/HTTPS with\n      authentication and encryption provided via certificate (preferred being SHA2).\"\n  - id: vendor-portal-login\n    type: http\n    subtype: session-login\n\
  \    surface: AceHardware-Vendors.com vendor portal\n    description: >-\n      The vendor portal at www.acehardware-vendors.com serves a public documents area (the Ace\n      Vendor Manual and forms are readable anonymously) behind which vendor-specific functions\n      require a portal account issued by Ace Hardware. No public registration path exists.\n    self_service: false\n    evidence: 'https://www.acehardware-vendors.com/ returned 200 with a public Vendors Public documents area and a login for vendor-specific functions (probed 2026-08-30).'\n  - id: impact-affiliate-account\n    type: delegated\n    subtype: third-party-network-account\n    surface: Ace Hardware Affiliate Program\n    description: >-\n      The affiliate program is operated on the Impact partner network. Tracking links, banners\n      and reporting are accessed with an Impact media-partner account, not with an Ace Hardware\n      credential. Any programmatic access to affiliate reporting is Impact's API under\
  \ Impact's\n      own credentials — Ace Hardware issues no affiliate API key.\n    self_service: true\n    signup: 'https://app.impact.com/campaign-mediapartner-signup/Ace-Hardware.brand?type=dm'\n    evidence: 'https://www.acehardware.com/affiliates states \"You can find reporting, links, and banners at Impact!\" and links the media-partner signup.'\n\nabsent:\n  - scheme: apiKey\n    note: No API key issuance, no key prefix, and no key management surface is documented.\n  - scheme: oauth2\n    note: '/.well-known/oauth-authorization-server returned 500 (empty) on www.acehardware.com and 404 on www.acehardware-vendors.com.'\n  - scheme: openIdConnect\n    note: '/.well-known/openid-configuration returned 500 (empty) on www.acehardware.com and 404 on www.acehardware-vendors.com.'\n  - scheme: bearer\n    note: No token endpoint or bearer-token documentation exists on either host.\n\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ace-hardware/refs/heads/main/authentication/ace-hardware-authentication.yml
summary_line: 3 schemes
tags:
- Retail
- Hardware
- Home Improvement
- Tools
- Paint
- Cooperative
- EDI
- Affiliates
---
