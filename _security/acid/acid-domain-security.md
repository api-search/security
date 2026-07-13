---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Google Spanner API
  slug: google-spanner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/APIs-guru/openapi-directory/main/APIs/googleapis.com/spanner/v1/openapi.yaml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 iodef "mailto:dns-admin@wikimedia.org"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wikipedia.org
  spf: true
- caa:
  - 0 iodef "mailto:hostmaster@postgresql.org"
  - 0 issue "amazontrust.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: postgresql.org
  spf: true
hosts:
- cert_expires: Sep  4 20:06:43 2026 GMT
  host: en.wikipedia.org
  hsts: true
  hsts_max_age: 106384710
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 17:09:46 2026 GMT
  host: www.postgresql.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 23:24:02 2026 GMT
  host: www.cockroachlabs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Acid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ACID, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ACID
provider_slug: acid
slug: acid-domain-security
source_filename: acid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: en.wikipedia.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 20:06:43 2026 GMT\n  hsts: true\n  hsts_max_age: 106384710\n- host: www.postgresql.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 17:09:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.cockroachlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 23:24:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wikipedia.org\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:dns-admin@wikimedia.org\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: postgresql.org\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:hostmaster@postgresql.org\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acid/refs/heads/main/security/acid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- ACID
- Database
- Transactions
- Atomicity
- Consistency
- Isolation
- Durability
- Distributed Systems
---
