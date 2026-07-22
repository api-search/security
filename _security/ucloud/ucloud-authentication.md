---
api_key_in: []
auth_types:
- signature
description: ''
kind: authentication
layout: security
method: searched
name: Ucloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: UCloud secures its APIs with signature across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: UCloud
provider_slug: ucloud
scheme_count: 2
schemes:
- controls:
  - IP allowlist for open-API calls configurable at console.ucloud.cn/uaccount/userinfo (applies to all sub-accounts)
  - IAM sub-accounts; RetCode 299 signals an IAM permission failure
  - ProjectId scoping (sub-accounts must always pass ProjectId)
  description: Every request carries the account PublicKey plus a Signature parameter. The signature is SHA1(concatenation of all request parameters sorted ascending by name, values appended without HTTP escaping, with the account PrivateKey appended at the end). Keys are issued per account in the UAPI console.
  endpoints:
  - https: true
    network: public
    url: https://api.ucloud.cn
  - https: false
    network: vpc-internal
    notes: In-VPC endpoint; HTTPS not supported; requires 10.10.10.10 in the account IP allowlist when one is configured.
    url: http://api.service.ucloud.cn
  key_console: https://console.ucloud.cn/uapi/apikey
  name: UCloudSignature
  required_parameters:
  - Action
  - PublicKey
  - Signature
  scoping_parameters:
  - Region
  - Zone
  - ProjectId
  type: signature
- description: The first-party ucloud CLI supports OAuth authorization (`ucloud auth login`, with --no-browser for headless environments) as the preferred way to initialize a profile, falling back to AK/SK (PublicKey/PrivateKey) profiles for scripts and CI/CD.
  docs: https://github.com/ucloud/skills/blob/main/ucloud-cli/SKILL.md
  name: CLIOAuth
  type: oauth2-interactive
slug: ucloud-authentication
source_filename: ucloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\ndocs: https://docs.ucloud.cn/api/summary/signature\nsource: https://docs.ucloud.cn/api/summary/signature + https://docs.ucloud.cn/api/summary/public\nnotes: >-\n  The UCloud Open API uses a proprietary request-signature scheme, not OAuth\n  or bearer tokens. There is no OpenAPI document to derive from; this profile\n  was captured from the published signature and quickstart docs. Interactive\n  CLI sessions can alternatively authenticate with an OAuth browser flow\n  (`ucloud auth login`), but raw API calls always use the signature scheme.\nsummary:\n  types: [signature]\n  transport: request parameters (query string or JSON/form body) over HTTPS GET/POST\n  oauth2_flows: []\nschemes:\n  - name: UCloudSignature\n    type: signature\n    description: >-\n      Every request carries the account PublicKey plus a Signature parameter.\n      The signature is SHA1(concatenation of all request parameters sorted\n      ascending by name, values\
  \ appended without HTTP escaping, with the\n      account PrivateKey appended at the end). Keys are issued per account in\n      the UAPI console.\n    key_console: https://console.ucloud.cn/uapi/apikey\n    required_parameters: [Action, PublicKey, Signature]\n    scoping_parameters: [Region, Zone, ProjectId]\n    endpoints:\n      - {url: 'https://api.ucloud.cn', network: public, https: true}\n      - {url: 'http://api.service.ucloud.cn', network: vpc-internal, https: false, notes: In-VPC endpoint; HTTPS not supported; requires 10.10.10.10 in the account IP allowlist when one is configured.}\n    controls:\n      - IP allowlist for open-API calls configurable at console.ucloud.cn/uaccount/userinfo (applies to all sub-accounts)\n      - IAM sub-accounts; RetCode 299 signals an IAM permission failure\n      - ProjectId scoping (sub-accounts must always pass ProjectId)\n  - name: CLIOAuth\n    type: oauth2-interactive\n    description: >-\n      The first-party ucloud CLI supports OAuth\
  \ authorization (`ucloud auth\n      login`, with --no-browser for headless environments) as the preferred\n      way to initialize a profile, falling back to AK/SK (PublicKey/PrivateKey)\n      profiles for scripts and CI/CD.\n    docs: https://github.com/ucloud/skills/blob/main/ucloud-cli/SKILL.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ucloud/refs/heads/main/authentication/ucloud-authentication.yml
summary_line: signature · 2 schemes
tags:
- Company
- Enterprise
- Cloud Computing
- IaaS
- GPU
- Kubernetes
- Object Storage
- CDN
- China
---
