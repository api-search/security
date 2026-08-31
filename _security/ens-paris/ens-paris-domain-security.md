---
description: ''
domains:
- caa:
  - 0 issuewild "harica.gr"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "harica.gr"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: psl.eu
  spf: true
- caa:
  - 0 issuewild "harica.gr"
  - 0 iodef "mailto:tcs@renater.fr"
  - 0 issue "harica.gr"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: renater.fr
  spf: true
hosts:
- cert_expires: Oct  9 13:05:10 2026 GMT
  host: www.ens.psl.eu
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 10:22:07 2026 GMT
  host: services.renater.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: federation.ens.psl.eu
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Ens Paris Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for École Normale Supérieure de Paris, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: École Normale Supérieure de Paris
provider_slug: ens-paris
slug: ens-paris-domain-security
source_filename: ens-paris-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ens.psl.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:05:10 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: services.renater.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 10:22:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: federation.ens.psl.eu\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: psl.eu\n  dnssec: false\n  caa:\n  - 0 issuewild \"harica.gr\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"harica.gr\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: renater.fr\n  dnssec: false\n  caa:\n  - 0 issuewild \"harica.gr\"\n  - 0 iodef \"\
  mailto:tcs@renater.fr\"\n  - 0 issue \"harica.gr\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ens-paris/refs/heads/main/security/ens-paris-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- University
- Higher Education
- Education
- France
- Université PSL
- Research
- Identity Federation
- Library
- Open Access
- OAI-PMH
---
