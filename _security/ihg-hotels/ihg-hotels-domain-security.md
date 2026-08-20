---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dmarc_reporting: rua to dmarcian and Proofpoint Email Defense; ruf to Proofpoint. fo=1.
  dnssec: false
  domain: ihg.com
  note: 'SPF is well-formed and ends in a hard fail (-all), which is the strong choice. DMARC is published but p=none: reports are collected and acted on by two vendors, but no receiver is instructed to quarantine or reject spoofed IHG mail. For a brand whose loyalty programme is a standing phishing target, p=none is the weak link.'
  spf: true
  spf_qualifier: -all
  spf_record: v=spf1 include:_spf.ihg.com include:_spf.google.com include:amazonses.com include:spf.protection.outlook.com include:_spf.highradius.com ip4:148.163.135.129 ip4:216.133.255.190 ip4:147.154.153.87 ip4:138.1.67.161 ip4:138.1.65.17 -all
- caa: []
  dmarc: false
  dnssec: false
  domain: ihgplc.com
  note: The investor-relations domain publishes neither SPF nor DMARC. Any sender can spoof @ihgplc.com with no policy signal to receivers.
  spf: false
hosts:
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: www.ihg.com
  hsts: false
  hsts_max_age: null
  https: true
  note: Consumer booking site. Akamai bot defence returns 403 to non-browser clients.
  server: AkamaiGHost
  tls_version: TLSv1.3
- cert_valid: true
  host: www.ihgplc.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15552000
  hsts_preload: true
  https: true
  note: Investis-hosted corporate site. The only IHG host with a strong HSTS policy.
  server: cloudflare
  tls_version: TLSv1.3
- cert_valid: true
  edge: prod-external.ihg.edgekey.net
  host: apis.ihg.com
  hsts: false
  http_status: 403
  https: true
  server: AkamaiGHost
  tls_version: TLSv1.3
- cert_valid: true
  edge: np-external.ihg.edgekey.net
  host: dev-apis.ihg.com
  hsts: false
  http_status: 403
  https: true
  note: Non-production external API edge, discovered this round.
  server: AkamaiGHost
  tls_version: TLSv1.3
- cert_valid: true
  edge: prod-b2b.ihg.edgekey.net
  host: b2b.ihg.com
  hsts: false
  http_status: 404
  https: true
  server: AkamaiNetStorage
  tls_version: TLSv1.3
- cert_valid: true
  host: partnerconnect.ihg.com
  hsts: false
  http_status: 200
  https: true
  note: The live affiliate programme, running WordPress 5.2.24 — a release line that has been out of active support for years. No HSTS.
  server: nginx
  tls_version: TLSv1.3
- cert_valid: true
  host: www.ihgagent.com
  hsts: false
  http_status: 403
  https: true
  note: Travel agent portal; redirects to www.ihg.com/agent-portal, then Akamai-blocked.
  server: AkamaiGHost
  tls_version: TLSv1.3
- host: api.ihg.com
  https: unknown
  note: Resolves through ihg.api.mashery.com and sb-ihg.mashery.com. The TLS connection times out from this client, so no transport assertion is made.
kind: domain-security
layout: security
method: probed
name: Ihg Hotels Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IHG Hotels & Resorts, probed live across 8 host(s) and 2 registrable domain(s). 8 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: IHG Hotels & Resorts
provider_slug: ihg-hotels
slug: ihg-hotels-domain-security
source_filename: ihg-hotels-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: probed\nsource: >-\n  live DNS/TLS/HTTP probes of apis.yml hosts plus every IHG API and edge\n  hostname found in review.yml. Baseline written by\n  0-working/probe-domain-security.py, extended with the additional hosts and\n  the ihgplc.com registrable domain. Probed 2026-07-28.\nsummary: >-\n  TLS hygiene is uniformly good — every IHG host that answers negotiates\n  TLS 1.3 with a valid certificate chain. Everything above the transport is\n  weak or missing. www.ihg.com, the consumer booking site that carries payment\n  and loyalty traffic, returns no HSTS header at all. The ihg.com DMARC record\n  is published but set to p=none, which monitors spoofing rather than\n  preventing it. Neither ihg.com nor ihgplc.com is DNSSEC-signed and neither\n  publishes a CAA record, so nothing constrains which CA may issue for these\n  domains. ihgplc.com — the investor-relations domain — publishes no SPF and no\n  DMARC record of any kind.\nhosts:\n- host:\
  \ www.ihg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: false\n  hsts_max_age: null\n  server: AkamaiGHost\n  note: Consumer booking site. Akamai bot defence returns 403 to non-browser clients.\n- host: www.ihgplc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_valid: true\n  hsts: true\n  hsts_max_age: 15552000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  server: cloudflare\n  note: Investis-hosted corporate site. The only IHG host with a strong HSTS policy.\n- host: apis.ihg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_valid: true\n  hsts: false\n  server: AkamaiGHost\n  http_status: 403\n  edge: prod-external.ihg.edgekey.net\n- host: dev-apis.ihg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_valid: true\n  hsts: false\n  server: AkamaiGHost\n  http_status: 403\n  edge: np-external.ihg.edgekey.net\n  note: Non-production external API edge, discovered this round.\n- host: b2b.ihg.com\n  https: true\n  tls_version:\
  \ TLSv1.3\n  cert_valid: true\n  hsts: false\n  server: AkamaiNetStorage\n  http_status: 404\n  edge: prod-b2b.ihg.edgekey.net\n- host: partnerconnect.ihg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_valid: true\n  hsts: false\n  server: nginx\n  http_status: 200\n  note: >-\n    The live affiliate programme, running WordPress 5.2.24 — a release line\n    that has been out of active support for years. No HSTS.\n- host: www.ihgagent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_valid: true\n  hsts: false\n  server: AkamaiGHost\n  http_status: 403\n  note: Travel agent portal; redirects to www.ihg.com/agent-portal, then Akamai-blocked.\n- host: api.ihg.com\n  https: unknown\n  note: >-\n    Resolves through ihg.api.mashery.com and sb-ihg.mashery.com. The TLS\n    connection times out from this client, so no transport assertion is made.\ndomains:\n- domain: ihg.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: >-\n    v=spf1 include:_spf.ihg.com include:_spf.google.com\
  \ include:amazonses.com\n    include:spf.protection.outlook.com include:_spf.highradius.com\n    ip4:148.163.135.129 ip4:216.133.255.190 ip4:147.154.153.87 ip4:138.1.67.161\n    ip4:138.1.65.17 -all\n  spf_qualifier: '-all'\n  dmarc: true\n  dmarc_policy: none\n  dmarc_reporting: >-\n    rua to dmarcian and Proofpoint Email Defense; ruf to Proofpoint. fo=1.\n  note: >-\n    SPF is well-formed and ends in a hard fail (-all), which is the strong\n    choice. DMARC is published but p=none: reports are collected and acted on\n    by two vendors, but no receiver is instructed to quarantine or reject\n    spoofed IHG mail. For a brand whose loyalty programme is a standing\n    phishing target, p=none is the weak link.\n- domain: ihgplc.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  note: >-\n    The investor-relations domain publishes neither SPF nor DMARC. Any sender\n    can spoof @ihgplc.com with no policy signal to receivers.\nsecurity_txt: false\nvulnerability_disclosure:\
  \ none-found\ntrust_center: false\ndisclosure_note: >-\n  0-working/probe-security-programs.py returned vdp=none trust=none on\n  2026-07-28. No /.well-known/security.txt on ihg.com (403 bot-block),\n  ihgplc.com (404) or partnerconnect.ihg.com (404). trust.ihg.com and\n  security.ihg.com do not resolve. No bug bounty programme on HackerOne,\n  Bugcrowd or Intigriti was found. No named certification (SOC 2, ISO 27001,\n  PCI DSS, HIPAA, FedRAMP) is published on any IHG property; the\n  responsible-business policy library carries environmental, human-rights,\n  community and supplier-code documents but no information-security policy.\n  Because nothing was verified, no VulnerabilityDisclosure, Security,\n  TrustCenter or Compliance pointer is wired into apis.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ihg-hotels/refs/heads/main/security/ihg-hotels-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- United Kingdom
- Hospitality
- Hotels
- Booking
- Distribution
- GDS
- Loyalty
- Affiliates
- Partner Gated
---
