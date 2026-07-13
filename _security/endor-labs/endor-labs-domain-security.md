---
api_specs:
- filename: endor-labs-openapi.yml
  format: yaml
  label: Endor Labs Projects API
  slug: endor-labs-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endor-labs/refs/heads/main/openapi/endor-labs-openapi.yml
- filename: endor-labs-openapi.yml
  format: yaml
  label: Endor Labs Dependencies & Packages API
  slug: endor-labs-dependencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endor-labs/refs/heads/main/openapi/endor-labs-openapi.yml
- filename: endor-labs-openapi.yml
  format: yaml
  label: Endor Labs Findings API
  slug: endor-labs-findings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endor-labs/refs/heads/main/openapi/endor-labs-openapi.yml
- filename: endor-labs-openapi.yml
  format: yaml
  label: Endor Labs Policies API
  slug: endor-labs-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endor-labs/refs/heads/main/openapi/endor-labs-openapi.yml
- filename: endor-labs-openapi.yml
  format: yaml
  label: Endor Labs Scan Results API
  slug: endor-labs-scan-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endor-labs/refs/heads/main/openapi/endor-labs-openapi.yml
- filename: endor-labs-openapi.yml
  format: yaml
  label: Endor Labs Auth & Namespaces API
  slug: endor-labs-auth-namespaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endor-labs/refs/heads/main/openapi/endor-labs-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: endorlabs.com
  spf: true
hosts:
- cert_expires: Aug 12 09:54:30 2026 GMT
  host: www.endorlabs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 10:27:54 2026 GMT
  host: docs.endorlabs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 11:44:38 2026 GMT
  host: api.endorlabs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Endor Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Endor Labs, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Endor Labs
provider_slug: endor-labs
slug: endor-labs-domain-security
source_filename: endor-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.endorlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 09:54:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.endorlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 10:27:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.endorlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 11:44:38 2026 GMT\n  hsts: null\ndomains:\n- domain: endorlabs.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/endor-labs/refs/heads/main/security/endor-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Security
- Software Supply Chain
- SCA
- Reachability
- AppSec
- AI Security
---
