---
api_specs:
- filename: singularitynet-marketplace-openapi.yml
  format: yaml
  label: SingularityNET Daemon API
  slug: singularitynet-daemon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singularity-net/refs/heads/main/openapi/singularitynet-marketplace-openapi.yml
- filename: singularitynet-marketplace-openapi.yml
  format: yaml
  label: SingularityNET Marketplace API
  slug: singularitynet-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singularity-net/refs/heads/main/openapi/singularitynet-marketplace-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: singularitynet.io
  spf: true
hosts:
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: dev.singularitynet.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: services.singularitynet.io
  https: false
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: marketplace.singularitynet.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Singularity Net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SingularityNET, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SingularityNET
provider_slug: singularity-net
slug: singularity-net-domain-security
source_filename: singularity-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dev.singularitynet.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: false\n- host: services.singularitynet.io\n  https: false\n- host: marketplace.singularitynet.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: singularitynet.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/singularity-net/refs/heads/main/security/singularity-net-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Blockchain
- Decentralized AI
- AI Marketplace
- Web3
---
