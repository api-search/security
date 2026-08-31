---
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
  dnssec: false
  domain: splitero.com
  spf: true
hosts:
- cert_expires: Oct  4 09:57:17 2026 GMT
  host: www.splitero.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 25 20:22:50 2026 GMT
  host: auth.splitero.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Stytch-backed authentication host (CNAME abundant-yogurt-9606.customers.stytch.com); serves /.well-known/jwks.json.
  tls_version: TLSv1.3
- cert_expires: Oct 13 13:06:32 2026 GMT
  host: my.splitero.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  note: Consumer portal on Vercel (app.splitero.com redirects here). All paths require login.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Splitero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Splitero, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Splitero
provider_slug: splitero
slug: splitero-domain-security
source_filename: splitero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts (probe-domain-security.py), extended with the two additional\n  splitero.com hosts found by DNS enumeration\nhosts:\n- host: www.splitero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 09:57:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: auth.splitero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 20:22:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: Stytch-backed authentication host (CNAME abundant-yogurt-9606.customers.stytch.com); serves /.well-known/jwks.json.\n- host: my.splitero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 13:06:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  note: Consumer portal on Vercel (app.splitero.com redirects here). All paths require login.\ndomains:\n- domain: splitero.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\
  \n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/splitero/refs/heads/main/security/splitero-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Fintech
- Real Estate
- Home Equity
- Lending
- Mortgage
- Consumer Finance
---
