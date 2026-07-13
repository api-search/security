---
api_specs:
- filename: freestyle-vm-api-openapi.yml
  format: yaml
  label: Freestyle VMs API
  slug: freestyle-vms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freestyle-sh/refs/heads/main/openapi/freestyle-vm-api-openapi.yml
- filename: freestyle-git-api-openapi.yml
  format: yaml
  label: Freestyle Git API
  slug: freestyle-git-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freestyle-sh/refs/heads/main/openapi/freestyle-git-api-openapi.yml
- filename: freestyle-identity-api-openapi.yml
  format: yaml
  label: Freestyle Identity API
  slug: freestyle-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freestyle-sh/refs/heads/main/openapi/freestyle-identity-api-openapi.yml
- filename: freestyle-domains-api-openapi.yml
  format: yaml
  label: Freestyle Domains API
  slug: freestyle-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freestyle-sh/refs/heads/main/openapi/freestyle-domains-api-openapi.yml
- filename: freestyle-execute-api-openapi.yml
  format: yaml
  label: Freestyle Execute API
  slug: freestyle-execute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freestyle-sh/refs/heads/main/openapi/freestyle-execute-api-openapi.yml
- filename: freestyle-web-api-openapi.yml
  format: yaml
  label: Freestyle Web Deployments API
  slug: freestyle-web-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freestyle-sh/refs/heads/main/openapi/freestyle-web-api-openapi.yml
- filename: freestyle-cron-api-openapi.yml
  format: yaml
  label: Freestyle Cron API
  slug: freestyle-cron-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freestyle-sh/refs/heads/main/openapi/freestyle-cron-api-openapi.yml
- filename: freestyle-observability-api-openapi.yml
  format: yaml
  label: Freestyle Observability API
  slug: freestyle-observability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freestyle-sh/refs/heads/main/openapi/freestyle-observability-api-openapi.yml
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
