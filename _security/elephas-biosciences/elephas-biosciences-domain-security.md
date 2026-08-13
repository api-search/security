---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: elephas.com
  note: DMARC policy is p=none — monitoring only, no enforcement against spoofed mail from the corporate domain.
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: elephasapis.com
  note: The API domain publishes neither SPF nor DMARC. It is an API-only domain that sends no mail, so the gap is low-impact, but a null SPF/DMARC record would close it explicitly.
  spf: false
hosts:
- cert_expires: Oct 28 10:08:57 2026 GMT
  host: elephas.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 17 23:59:59 2026 GMT
  cert_issuer: Sectigo Public Server Authentication CA DV R36
  chain_complete: false
  chain_note: openssl s_client verify return code 21 (unable to verify the first certificate) — the server presents the leaf without its Sectigo intermediate. Browsers and curl recover via AIA fetching, but strict clients (Python ssl with the system store, some JVM and Go clients, many API gateways) fail the handshake. This is a real, fixable server misconfiguration, not a probe artifact.
  host: portal.elephas.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 16 23:59:59 2027 GMT
  cert_issuer: Sectigo Public Server Authentication CA DV R36
  chain_complete: false
  chain_note: Same incomplete chain as portal.elephas.com — leaf served without the Sectigo intermediate.
  host: portal.elephasapis.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 16 23:59:59 2026 GMT
  cert_issuer: GeoTrust TLS RSA CA G1 (DigiCert)
  chain_complete: true
  host: na.login.elephas.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Azure AD B2C custom-domain identity host for the Elephas tenant.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Elephas Biosciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elephas Biosciences, probed live across 4 host(s) and 2 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Elephas Biosciences
provider_slug: elephas-biosciences
slug: elephas-biosciences-domain-security
source_filename: elephas-biosciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts (probe-domain-security.py, then\n  corrected by hand with openssl s_client + curl -I where the automated TLS probe\n  failed on chain resolution)\nhosts:\n- host: elephas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 10:08:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: portal.elephas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Sectigo Public Server Authentication CA DV R36\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  chain_complete: false\n  chain_note: 'openssl s_client verify return code 21 (unable to verify the first\n    certificate) — the server presents the leaf without its Sectigo intermediate.\n    Browsers and curl recover via AIA fetching, but strict clients (Python ssl with\n    the system store, some JVM and Go clients, many API gateways) fail the\n    handshake. This is a real, fixable server misconfiguration, not a probe\
  \ artifact.'\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: portal.elephasapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Sectigo Public Server Authentication CA DV R36\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  chain_complete: false\n  chain_note: Same incomplete chain as portal.elephas.com — leaf served without the\n    Sectigo intermediate.\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: na.login.elephas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: GeoTrust TLS RSA CA G1 (DigiCert)\n  cert_expires: Nov 16 23:59:59 2026 GMT\n  chain_complete: true\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: Azure AD B2C custom-domain identity host for the Elephas tenant.\ndomains:\n- domain: elephas.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  note: 'DMARC policy is p=none — monitoring only, no enforcement against spoofed\n\
  \    mail from the corporate domain.'\n- domain: elephasapis.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  note: 'The API domain publishes neither SPF nor DMARC. It is an API-only domain\n    that sends no mail, so the gap is low-impact, but a null SPF/DMARC record would\n    close it explicitly.'\nresponse_security_headers:\n  observed_on: https://portal.elephasapis.com/swagger\n  headers:\n  - strict-transport-security: max-age=31536000;includeSubdomains\n  - x-content-type-options: nosniff\n  - content-security-policy: frame-ancestors 'none'\n  - referrer-policy: no-referrer\n  - cache-control: no-store, max-age=0, no-transform\n  - permissions-policy: geolocation=(self \"https://portal.elephas.com\"\n      \"https://portal.elephasapis.com\")\n  note: The API returns a solid, deliberately configured security-header set on\n    unauthenticated responses.\nfindings:\n- id: incomplete-tls-chain\n  severity: medium\n  hosts: [portal.elephas.com, portal.elephasapis.com]\n\
  \  detail: Leaf certificate served without its issuing intermediate; strict TLS\n    clients cannot build a path to a trusted root.\n- id: no-caa-records\n  severity: low\n  domains: [elephas.com, elephasapis.com]\n  detail: No CAA records, so any public CA may issue for these names.\n- id: dmarc-not-enforcing\n  severity: low\n  domains: [elephas.com]\n  detail: DMARC exists but is p=none.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elephas-biosciences/refs/heads/main/security/elephas-biosciences-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Life Sciences
- Biotechnology
- Precision Oncology
- Diagnostics
- Immunotherapy
- Clinical Research
- Laboratory
- Medical Devices
---
