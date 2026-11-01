---
description: ''
domains:
- caa:
  - 0 issue "visa.com"
  - 0 issuewild ";"
  - 0 issue "digicert.com; account=34598d5fd7c7c32362dbd871f3557ebac0d69f11f52eca62212aa083919dd593"
  - 0 iodef "mailto:domainadmin@usbank.com"
  - 0 issue "entrust.net"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: elavon.com
  spf: true
hosts:
- cert_expires: Feb 15 23:59:59 2027 GMT
  host: www.elavon.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Elavon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elavon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Elavon
provider_slug: elavon
slug: elavon-domain-security
source_filename: elavon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.elavon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 15 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: elavon.com\n  dnssec: false\n  caa:\n  - 0 issue \"visa.com\"\n  - 0 issuewild \";\"\n  - 0 issue \"digicert.com; account=34598d5fd7c7c32362dbd871f3557ebac0d69f11f52eca62212aa083919dd593\"\n  - 0 iodef \"mailto:domainadmin@usbank.com\"\n  - 0 issue \"entrust.net\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/elavon/security/elavon-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Payments
- Merchant Services
- FinTech
- API
---
