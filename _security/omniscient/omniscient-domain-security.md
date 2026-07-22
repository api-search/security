---
description: ''
domains:
- caa:
  - ambitious-pond-05ed89703.4.azurestaticapps.net.
  - azurestaticappstm4.trafficmanager.net.
  - msha-slice-4-eus2-0.msha-slice-4-eus2-0-ase.p.azurewebsites.net.
  - waws-prod-bn1-1603b4fd.sip.p.azurewebsites.windows.net.
  dmarc: false
  dnssec: true
  domain: omniscient.so
  spf: true
hosts:
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: omniscient.so
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Omniscient Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Omniscient, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Omniscient
provider_slug: omniscient
slug: omniscient-domain-security
source_filename: omniscient-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: omniscient.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: omniscient.so\n  dnssec: true\n  caa:\n  - ambitious-pond-05ed89703.4.azurestaticapps.net.\n  - azurestaticappstm4.trafficmanager.net.\n  - msha-slice-4-eus2-0.msha-slice-4-eus2-0-ase.p.azurewebsites.net.\n  - waws-prod-bn1-1603b4fd.sip.p.azurewebsites.windows.net.\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/omniscient/refs/heads/main/security/omniscient-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Artificial Intelligence
- Risk Intelligence
- Reputation Monitoring
- Geopolitical Risk
- ESG
- Decision Intelligence
---
