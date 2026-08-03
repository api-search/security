---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: thayermahan.com
  spf: true
hosts:
- cert_expires: Oct 16 14:53:00 2026 GMT
  host: www.thayermahan.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thayermahan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ThayerMahan, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ThayerMahan
provider_slug: thayermahan
slug: thayermahan-domain-security
source_filename: thayermahan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thayermahan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 14:53:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: thayermahan.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thayermahan/refs/heads/main/security/thayermahan-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Defense
- Maritime
- Ocean Intelligence
- Autonomous Systems
- Undersea Surveillance
- Passive Acoustics
- Critical Infrastructure
- Port Security
- Uncrewed Surface Vessels
- Marine Mammal Monitoring
- National Security
---
