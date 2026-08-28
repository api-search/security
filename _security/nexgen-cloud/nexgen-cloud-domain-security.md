---
api_specs:
- filename: nexgen-cloud-hyperstack-openapi.json
  format: json
  label: Hyperstack API
  slug: nexgen-cloud-hyperstack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexgen-cloud/refs/heads/main/openapi/nexgen-cloud-hyperstack-openapi.json
- filename: nexgen-cloud-ai-studio-openapi.json
  format: json
  label: Hyperstack AI Studio API
  slug: nexgen-cloud-ai-studio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexgen-cloud/refs/heads/main/openapi/nexgen-cloud-ai-studio-openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nexgencloud.com
  spf: true
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: hyperstack.cloud
  spf: true
hosts:
- cert_expires: Oct 26 18:51:27 2026 GMT
  host: www.nexgencloud.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 22 14:15:22 2026 GMT
  host: docs.hyperstack.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 10:42:06 2026 GMT
  host: infrahub-api.nexgencloud.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nexgen Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NexGen Cloud, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: NexGen Cloud
provider_slug: nexgen-cloud
slug: nexgen-cloud-domain-security
source_filename: nexgen-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nexgencloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 18:51:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.hyperstack.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 14:15:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: infrahub-api.nexgencloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 10:42:06 2026 GMT\n  hsts: null\ndomains:\n- domain: nexgencloud.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: hyperstack.cloud\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com\"\n \
  \ - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexgen-cloud/refs/heads/main/security/nexgen-cloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cloud
- GPU
- Artificial Intelligence
- Machine Learning
- Infrastructure
- Compute
- Kubernetes
- Storage
- Inference
- Virtual Machines
- Sovereign AI
---
