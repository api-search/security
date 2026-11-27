---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:dnsmaster@dataart.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dataart.com
  spf: true
hosts:
- cert_expires: Jan 25 04:16:46 2027 GMT
  host: dataart.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DataArt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DataArt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DataArt
provider_slug: dataart-com
slug: dataart-com-domain-security
source_filename: dataart-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dataart.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 25 04:16:46 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dataart.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:dnsmaster@dataart.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/dataart-com/security/dataart-com-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Artificial Intelligence
- Consulting
- Software Development
- Data Engineering
- Enterprise
---
