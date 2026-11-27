---
description: ''
domains:
- caa:
  - 0 issuewild "globalsign.com"
  - 0 issue "globalsign.com"
  - 0 issue "trustproviderbv.digitalcertvalidation.com"
  - 0 issuewild "trustproviderbv.digitalcertvalidation.com"
  - 0 iodef "security.caa@boursedirect.fr"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: boursedirect.fr
  spf: true
hosts:
- cert_expires: Mar 11 13:12:46 2027 GMT
  host: www.boursedirect.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bourse Direct Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bourse Direct, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bourse Direct
provider_slug: boursedirect
slug: boursedirect-domain-security
source_filename: boursedirect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.boursedirect.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 11 13:12:46 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: boursedirect.fr\n  dnssec: false\n  caa:\n  - 0 issuewild \"globalsign.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"trustproviderbv.digitalcertvalidation.com\"\n  - 0 issuewild \"trustproviderbv.digitalcertvalidation.com\"\n  - 0 iodef \"security.caa@boursedirect.fr\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/boursedirect/security/boursedirect-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Finance
- Brokerage
- Trading
- France
---
