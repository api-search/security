---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: esipfed.org
  spf: true
hosts:
- cert_expires: Nov 24 22:04:52 2026 GMT
  host: www.esipfed.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Earth Science Information Partners Esip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Earth Science Information Partners (ESIP), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Earth Science Information Partners (ESIP)
provider_slug: earth-science-information-partners-esip
slug: earth-science-information-partners-esip-domain-security
source_filename: earth-science-information-partners-esip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.esipfed.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 22:04:52 2026 GMT\n  hsts: false\ndomains:\n- domain: esipfed.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/earth-science-information-partners-esip/security/earth-science-information-partners-esip-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
