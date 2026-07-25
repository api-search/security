---
api_specs:
- filename: spacemesh-accountservice-api-openapi.yml
  format: yaml
  label: Spacemesh AccountService API
  slug: spacemesh-accountservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacemesh/refs/heads/main/openapi/spacemesh-accountservice-api-openapi.yml
- filename: spacemesh-activationservice-api-openapi.yml
  format: yaml
  label: Spacemesh ActivationService API
  slug: spacemesh-activationservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacemesh/refs/heads/main/openapi/spacemesh-activationservice-api-openapi.yml
- filename: spacemesh-layerservice-api-openapi.yml
  format: yaml
  label: Spacemesh LayerService API
  slug: spacemesh-layerservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacemesh/refs/heads/main/openapi/spacemesh-layerservice-api-openapi.yml
- filename: spacemesh-malfeasanceservice-api-openapi.yml
  format: yaml
  label: Spacemesh MalfeasanceService API
  slug: spacemesh-malfeasanceservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacemesh/refs/heads/main/openapi/spacemesh-malfeasanceservice-api-openapi.yml
- filename: spacemesh-networkservice-api-openapi.yml
  format: yaml
  label: Spacemesh NetworkService API
  slug: spacemesh-networkservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacemesh/refs/heads/main/openapi/spacemesh-networkservice-api-openapi.yml
- filename: spacemesh-nodeservice-api-openapi.yml
  format: yaml
  label: Spacemesh NodeService API
  slug: spacemesh-nodeservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacemesh/refs/heads/main/openapi/spacemesh-nodeservice-api-openapi.yml
- filename: spacemesh-rewardservice-api-openapi.yml
  format: yaml
  label: Spacemesh RewardService API
  slug: spacemesh-rewardservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacemesh/refs/heads/main/openapi/spacemesh-rewardservice-api-openapi.yml
- filename: spacemesh-transactionservice-api-openapi.yml
  format: yaml
  label: Spacemesh TransactionService API
  slug: spacemesh-transactionservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacemesh/refs/heads/main/openapi/spacemesh-transactionservice-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: spacemesh.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: spacemesh.network
  spf: true
hosts:
- host: spacemesh.io
  https: false
- cert_expires: Sep 29 22:02:33 2026 GMT
  host: testnet-api.spacemesh.network
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spacemesh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spacemesh, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Spacemesh
provider_slug: spacemesh
slug: spacemesh-domain-security
source_filename: spacemesh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spacemesh.io\n  https: false\n- host: testnet-api.spacemesh.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 22:02:33 2026 GMT\n  hsts: false\ndomains:\n- domain: spacemesh.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: spacemesh.network\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spacemesh/refs/heads/main/security/spacemesh-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Crypto Infrastructure
- Blockchain
- Cryptocurrency
- Proof of Space-Time
- Layer 1
- gRPC
- Node API
- Open Source
---
