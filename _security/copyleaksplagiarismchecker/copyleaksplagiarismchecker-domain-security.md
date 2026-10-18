---
api_specs:
- filename: copyleaksplagiarismchecker-ai-image-detector-async-api-openapi.yml
  format: yaml
  label: Copyleaksplagiarismchecker Ai Image Detector Async API
  slug: copyleaksplagiarismchecker-ai-image-detector-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copyleaksplagiarismchecker/refs/heads/main/openapi/copyleaksplagiarismchecker-ai-image-detector-async-api-openapi.yml
- filename: copyleaksplagiarismchecker-ai-video-detector-api-openapi.yml
  format: yaml
  label: Copyleaksplagiarismchecker Ai Video Detector API
  slug: copyleaksplagiarismchecker-ai-video-detector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copyleaksplagiarismchecker/refs/heads/main/openapi/copyleaksplagiarismchecker-ai-video-detector-api-openapi.yml
- filename: copyleaksplagiarismchecker-downloads-api-openapi.yml
  format: yaml
  label: Copyleaksplagiarismchecker Downloads API
  slug: copyleaksplagiarismchecker-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copyleaksplagiarismchecker/refs/heads/main/openapi/copyleaksplagiarismchecker-downloads-api-openapi.yml
- filename: copyleaksplagiarismchecker-my-scan-123-api-openapi.yml
  format: yaml
  label: Copyleaksplagiarismchecker My Scan 123 API
  slug: copyleaksplagiarismchecker-my-scan-123-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copyleaksplagiarismchecker/refs/heads/main/openapi/copyleaksplagiarismchecker-my-scan-123-api-openapi.yml
- filename: copyleaksplagiarismchecker-repositories-api-openapi.yml
  format: yaml
  label: Copyleaksplagiarismchecker Repositories API
  slug: copyleaksplagiarismchecker-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copyleaksplagiarismchecker/refs/heads/main/openapi/copyleaksplagiarismchecker-repositories-api-openapi.yml
- filename: copyleaksplagiarismchecker-scans-api-openapi.yml
  format: yaml
  label: Copyleaksplagiarismchecker Scans API
  slug: copyleaksplagiarismchecker-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copyleaksplagiarismchecker/refs/heads/main/openapi/copyleaksplagiarismchecker-scans-api-openapi.yml
- filename: copyleaksplagiarismchecker-writer-detector-api-openapi.yml
  format: yaml
  label: Copyleaksplagiarismchecker Writer Detector API
  slug: copyleaksplagiarismchecker-writer-detector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copyleaksplagiarismchecker/refs/heads/main/openapi/copyleaksplagiarismchecker-writer-detector-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "cloudflare.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: copyleaks.com
  spf: true
hosts:
- cert_expires: Dec 18 11:05:04 2026 GMT
  host: copyleaks.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Copyleaksplagiarismchecker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Copyleaksplagiarismchecker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Copyleaksplagiarismchecker
provider_slug: copyleaksplagiarismchecker
slug: copyleaksplagiarismchecker-domain-security
source_filename: copyleaksplagiarismchecker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: copyleaks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 11:05:04 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: copyleaks.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"cloudflare.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/copyleaksplagiarismchecker/refs/heads/main/security/copyleaksplagiarismchecker-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Detection
- Plagiarism Checker
- Content Integrity
- Education
- Enterprise
- Media Publishing
- API Integration
---
