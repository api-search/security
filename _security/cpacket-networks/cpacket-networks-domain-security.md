---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: cpacket.com
  spf: true
hosts:
- cert_expires: Dec 16 18:02:54 2026 GMT
  host: www.cpacket.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cpacket Networks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for cPacket Networks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: cPacket Networks
provider_slug: cpacket-networks
slug: cpacket-networks-domain-security
source_filename: cpacket-networks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cpacket.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 18:02:54 2026 GMT\n  hsts: false\ndomains:\n- domain: cpacket.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cpacket-networks/refs/heads/main/security/cpacket-networks-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Network Observability
- Packet Broker
- Artificial Intelligence
- Cloud
---
