---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:security@immunai.com"
  - 0 issue "amazon.com"
  - 0 issue "awstrust.com"
  - 0 issuewild "digicert.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: immunai.com
  spf: true
hosts:
- cert_expires: Sep  7 23:59:59 2026 GMT
  host: www.immunai.com
  hsts: null
  https: true
  note: No Strict-Transport-Security response header. Served by Flywheel/5.1.0 (managed WordPress hosting).
  tls_version: TLSv1.3
- cert_expires: null
  dns: 34.110.128.250
  host: api.immunai.com
  hsts: null
  http_status: null
  https: false
  note: An A record exists but no Immunai service answers on it. TCP 443 connects to a Google Cloud front end, then the TLS handshake is reset before any certificate is presented (no peer certificate available). Port 80 does not answer either. This is a stale DNS record pointing at a Google Cloud address that no longer terminates for this hostname — not an Immunai API host.
  tls_version: null
- cert_expires: Aug 26 23:59:59 2026 GMT
  dns: 34.144.219.193
  host: app.immunai.com
  hsts: null
  http_status: 403
  https: false
  note: An A record exists but the address is not serving Immunai. TLS completes and presents a certificate for an unrelated third party — subject CN=*.asa.com.br, issued by ZeroSSL — so the hostname fails certificate validation for any client. Ignoring validation, the Google Cloud front end returns 403 Forbidden. This is a dangling DNS record aimed at a Google Cloud address now held by another tenant.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Immunai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Immunai, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Immunai
provider_slug: immunai
slug: immunai-domain-security
source_filename: immunai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.immunai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 23:59:59 2026 GMT\n  hsts: null\n  note: >-\n    No Strict-Transport-Security response header. Served by Flywheel/5.1.0 (managed\n    WordPress hosting).\n- host: api.immunai.com\n  https: false\n  tls_version: null\n  cert_expires: null\n  hsts: null\n  dns: 34.110.128.250\n  http_status: null\n  note: >-\n    An A record exists but no Immunai service answers on it. TCP 443 connects to a\n    Google Cloud front end, then the TLS handshake is reset before any certificate is\n    presented (no peer certificate available). Port 80 does not answer either. This is\n    a stale DNS record pointing at a Google Cloud address that no longer terminates for\n    this hostname — not an Immunai API host.\n- host: app.immunai.com\n  https: false\n  tls_version: TLSv1.3\n  cert_expires: Aug 26\
  \ 23:59:59 2026 GMT\n  hsts: null\n  dns: 34.144.219.193\n  http_status: 403\n  note: >-\n    An A record exists but the address is not serving Immunai. TLS completes and\n    presents a certificate for an unrelated third party — subject CN=*.asa.com.br,\n    issued by ZeroSSL — so the hostname fails certificate validation for any client.\n    Ignoring validation, the Google Cloud front end returns 403 Forbidden. This is a\n    dangling DNS record aimed at a Google Cloud address now held by another tenant.\ndomains:\n- domain: immunai.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@immunai.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\nfindings:\n- id: dangling-dns-records\n  severity: informational\n  hosts:\n  - api.immunai.com\n  - app.immunai.com\n  summary: >-\n    Two immunai.com subdomains publish A records\
  \ into Google Cloud address space where\n    no Immunai service is reachable. app.immunai.com presents a valid certificate for a\n    wholly unrelated domain (*.asa.com.br), which is the signature of an address\n    released back to the cloud provider and reallocated to another tenant while the DNS\n    record was left in place. Recorded as observed fact; no exploitation was attempted\n    and no takeover is asserted.\n  observed: '2026-08-04'\n- id: no-hsts\n  severity: informational\n  hosts:\n  - www.immunai.com\n  summary: >-\n    The primary web host does not send Strict-Transport-Security, so it does not opt\n    into HSTS preloading or protect against a first-request downgrade.\n  observed: '2026-08-04'\n- id: no-dnssec\n  severity: informational\n  hosts:\n  - immunai.com\n  summary: The immunai.com zone is not DNSSEC signed.\n  observed: '2026-08-04'\nstrengths:\n- CAA is published and pins issuance to Let's Encrypt, Amazon and DigiCert.\n- CAA carries an iodef reporting address\
  \ (security@immunai.com) for certificate misissuance.\n- SPF is published and DMARC is enforced at policy p=reject.\n- TLS 1.3 on the primary web host.\nx-evidence:\n  fetched: '2026-08-04'\n  method: dig for DNS/CAA/SPF/DMARC; openssl s_client for TLS; curl for HTTP status and headers\n  note: >-\n    api.immunai.com and app.immunai.com were recorded as unresolved by the prior\n    enrichment round. They do resolve; this round probed them directly and recorded the\n    real state. Neither serves an Immunai API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/immunai/refs/heads/main/security/immunai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Immunology
- Drug Discovery
- Artificial Intelligence
- Machine Learning
- Single-Cell Genomics
- Multiomics
- Clinical Trials
- Life Sciences
---
