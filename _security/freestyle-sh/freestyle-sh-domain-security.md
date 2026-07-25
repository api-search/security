---
api_specs:
- filename: freestyle-sh-auth-api-openapi.yml
  format: yaml
  label: Freestyle Auth API
  slug: freestyle-sh-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freestyle-sh/refs/heads/main/openapi/freestyle-sh-auth-api-openapi.yml
- filename: freestyle-sh-certs-api-openapi.yml
  format: yaml
  label: Freestyle Certs API
  slug: freestyle-sh-certs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freestyle-sh/refs/heads/main/openapi/freestyle-sh-certs-api-openapi.yml
- filename: freestyle-sh-cron-api-openapi.yml
  format: yaml
  label: Freestyle Cron API
  slug: freestyle-sh-cron-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freestyle-sh/refs/heads/main/openapi/freestyle-sh-cron-api-openapi.yml
- filename: freestyle-sh-dns-api-openapi.yml
  format: yaml
  label: Freestyle DNS API
  slug: freestyle-sh-dns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freestyle-sh/refs/heads/main/openapi/freestyle-sh-dns-api-openapi.yml
- filename: freestyle-sh-domains-api-openapi.yml
  format: yaml
  label: Freestyle Domains API
  slug: freestyle-sh-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freestyle-sh/refs/heads/main/openapi/freestyle-sh-domains-api-openapi.yml
- filename: freestyle-sh-execute-api-openapi.yml
  format: yaml
  label: Freestyle Execute API
  slug: freestyle-sh-execute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freestyle-sh/refs/heads/main/openapi/freestyle-sh-execute-api-openapi.yml
- filename: freestyle-sh-git-api-openapi.yml
  format: yaml
  label: Freestyle Git API
  slug: freestyle-sh-git-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freestyle-sh/refs/heads/main/openapi/freestyle-sh-git-api-openapi.yml
- filename: freestyle-sh-identity-api-openapi.yml
  format: yaml
  label: Freestyle Identity API
  slug: freestyle-sh-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freestyle-sh/refs/heads/main/openapi/freestyle-sh-identity-api-openapi.yml
- filename: freestyle-sh-observability-api-openapi.yml
  format: yaml
  label: Freestyle Observability API
  slug: freestyle-sh-observability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freestyle-sh/refs/heads/main/openapi/freestyle-sh-observability-api-openapi.yml
- filename: freestyle-sh-vm-api-openapi.yml
  format: yaml
  label: Freestyle VM API
  slug: freestyle-sh-vm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freestyle-sh/refs/heads/main/openapi/freestyle-sh-vm-api-openapi.yml
- filename: freestyle-sh-web-api-openapi.yml
  format: yaml
  label: Freestyle Web API
  slug: freestyle-sh-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freestyle-sh/refs/heads/main/openapi/freestyle-sh-web-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: freestyle.sh
  spf: true
hosts:
- cert_expires: Sep 23 21:32:22 2026 GMT
  host: www.freestyle.sh
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 02:54:22 2026 GMT
  host: docs.freestyle.sh
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 27 18:07:26 2026 GMT
  host: api.freestyle.sh
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Freestyle Sh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Freestyle, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Freestyle
provider_slug: freestyle-sh
slug: freestyle-sh-domain-security
source_filename: freestyle-sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.freestyle.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 21:32:22 2026 GMT\n  hsts: false\n- host: docs.freestyle.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 02:54:22 2026 GMT\n  hsts: false\n- host: api.freestyle.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 27 18:07:26 2026 GMT\n  hsts: false\ndomains:\n- domain: freestyle.sh\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freestyle-sh/refs/heads/main/security/freestyle-sh-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- Agents
- Sandboxes
- VMs
- MicroVMs
- Git
- Code Execution
- JavaScript
- TypeScript
- Serverless
- Hosting
- Developer Tools
- Infrastructure
---
