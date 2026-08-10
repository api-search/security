---
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:security@getjerry.com"
  dmarc: true
  dmarc_pct: 100
  dmarc_policy: quarantine
  dmarc_rua: mailto:dmarc-reports@jerry.ai
  dnssec: true
  domain: jerry.ai
  spf: true
  spf_record: v=spf1 include:sendgrid.net include:_spf.google.com ~all
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:security@getjerry.com"
  dmarc: true
  dmarc_pct: 100
  dmarc_policy: quarantine
  dmarc_rua: mailto:dmarc-reports@getjerry.com
  dnssec: true
  domain: getjerry.com
  spf: true
  spf_record: v=spf1 include:sendgrid.net include:_spf.google.com ~all
hosts:
- cert_expires: Mar  1 23:59:59 2027 GMT
  host: jerry.ai
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  1 23:59:59 2027 GMT
  host: getjerry.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  note: 301-redirects to jerry.ai for site paths, but is the OIDC `issuer` value and serves /.well-known/openid-configuration and /.well-known/jwks.json.
  tls_version: TLSv1.3
- cert_expires: Oct 25 00:34:48 2026 GMT
  host: status.jerry.ai
  hsts: false
  https: true
  note: GitHub Pages (getjerry.github.io) — no HSTS header served.
  tls_version: TLSv1.3
- cert_expires: Oct 21 16:15:27 2026 GMT
  host: trust.jerry.ai
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: false
  https: true
  note: Vanta-hosted trust center (CNAME to cname.vantatrust.com).
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jerry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jerry, probed live across 4 host(s) and 2 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Jerry
provider_slug: jerry
slug: jerry-domain-security
source_filename: jerry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of every Jerry host reachable from apis.yml\nhosts:\n- host: jerry.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n- host: getjerry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  note: 301-redirects to jerry.ai for site paths, but is the OIDC `issuer` value and\n    serves /.well-known/openid-configuration and /.well-known/jwks.json.\n- host: status.jerry.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 00:34:48 2026 GMT\n  hsts: false\n  note: GitHub Pages (getjerry.github.io) — no HSTS header served.\n- host: trust.jerry.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 16:15:27 2026 GMT\n  hsts: true\n\
  \  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: false\n  note: Vanta-hosted trust center (CNAME to cname.vantatrust.com).\ndomains:\n- domain: jerry.ai\n  dnssec: true\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:security@getjerry.com\"\n  spf: true\n  spf_record: v=spf1 include:sendgrid.net include:_spf.google.com ~all\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_pct: 100\n  dmarc_rua: mailto:dmarc-reports@jerry.ai\n- domain: getjerry.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:security@getjerry.com\"\n  spf: true\n  spf_record: v=spf1 include:sendgrid.net include:_spf.google.com ~all\n  dmarc: true\n  dmarc_policy:\
  \ quarantine\n  dmarc_pct: 100\n  dmarc_rua: mailto:dmarc-reports@getjerry.com\nsummary:\n  strong:\n  - DNSSEC signed on both registrable domains\n  - HSTS with includeSubDomains and preload on both apex domains\n  - TLS 1.3 everywhere with valid chains\n  - CAA issue restrictions plus an iodef incident-reporting address\n  - SPF and enforced DMARC on both domains\n  gaps:\n  - DMARC policy is p=quarantine, not p=reject\n  - No HSTS on the status.jerry.ai GitHub Pages host\n  - No /.well-known/security.txt on any host (see jerry-vulnerability-disclosure.yml)\nx-evidence:\n  fetched: '2026-08-04'\n  method: dig (DS/CAA/TXT) + openssl s_client + HTTP HEAD\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jerry/refs/heads/main/security/jerry-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Insurance
- InsurTech
- Auto Insurance
- Insurance Broker
- Automotive
- Consumer Finance
- Lending
- Telematics
- Mobile Applications
- Artificial Intelligence
---
