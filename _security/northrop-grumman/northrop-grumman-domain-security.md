---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: northropgrumman.com
  note: TXT records present but none is a v=spf1 policy; _dmarc.northropgrumman.com returns NXDOMAIN (DNS status 3). No CAA records published.
  resolves: true
  role: public website
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dmarc_record: v=DMARC1; p=quarantine; fo=1; rua=mailto:dmarc_rua@ngc.com; ruf=mailto:dmarc_ruf@ngc.com
  dnssec: false
  domain: ngc.com
  resolves: true
  role: corporate mail domain; 301s to www.northropgrumman.com
  spf: true
  spf_record: v=spf1 exists:%{i}.spf.ngc.iphmx.com -all
- caa: []
  dmarc: false
  dnssec: false
  domain: northgrum.com
  resolves: true
  role: authoritative nameserver domain (sunrise/sundown/po/dnsdal.northgrum.com)
  spf: true
  spf_record: v=spf1 exists:%{i}.spf.ngc.iphmx.com -all
- dns_status: NXDOMAIN
  domain: northrop-grumman.com
  note: Probed because the previous apis.yml Website pointer used this hyphenated form. It has no A record and no nameservers; the pointer was dead and has been corrected to https://www.northropgrumman.com/.
  resolves: false
  role: not owned / not delegated
hosts:
- cert_expires: Nov 18 06:23:39 2026 GMT
  host: www.northropgrumman.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Northrop Grumman Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Northrop Grumman, probed live across 1 host(s) and 4 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Northrop Grumman
provider_slug: northrop-grumman
slug: northrop-grumman-domain-security
source_filename: northrop-grumman-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts (DoH via cloudflare-dns.com; TLS/HSTS via HTTPS handshake)\nnote: >-\n  Northrop Grumman splits its web identity from its mail identity. The public web domain\n  northropgrumman.com carries no SPF, no DMARC, no CAA and no DNSSEC, while the corporate\n  mail domain ngc.com — which redirects to the same website — carries both an SPF record\n  and a DMARC policy at p=quarantine. northgrum.com (the authoritative nameserver domain)\n  carries SPF but no DMARC. The hyphenated domain northrop-grumman.com, which this\n  profile previously pointed at, does not resolve at all (NXDOMAIN).\nhosts:\n- host: www.northropgrumman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 06:23:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: northropgrumman.com\n  role: public website\n  resolves: true\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  note:\
  \ >-\n    TXT records present but none is a v=spf1 policy; _dmarc.northropgrumman.com returns\n    NXDOMAIN (DNS status 3). No CAA records published.\n- domain: ngc.com\n  role: corporate mail domain; 301s to www.northropgrumman.com\n  resolves: true\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 exists:%{i}.spf.ngc.iphmx.com -all'\n  dmarc: true\n  dmarc_record: 'v=DMARC1; p=quarantine; fo=1; rua=mailto:dmarc_rua@ngc.com; ruf=mailto:dmarc_ruf@ngc.com'\n  dmarc_policy: quarantine\n- domain: northgrum.com\n  role: authoritative nameserver domain (sunrise/sundown/po/dnsdal.northgrum.com)\n  resolves: true\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 exists:%{i}.spf.ngc.iphmx.com -all'\n  dmarc: false\n- domain: northrop-grumman.com\n  role: not owned / not delegated\n  resolves: false\n  dns_status: NXDOMAIN\n  note: >-\n    Probed because the previous apis.yml Website pointer used this hyphenated form. It has\n    no A record and no nameservers; the pointer\
  \ was dead and has been corrected to\n    https://www.northropgrumman.com/.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/northrop-grumman/refs/heads/main/security/northrop-grumman-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Aerospace
- Autonomous Systems
- Command and Control
- Cybersecurity
- Defense
- Fortune 100
- Fortune 500
- Government
- Manufacturing
- Mission Systems
- Space
---
