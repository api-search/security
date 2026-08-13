---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ec.ai
  mx: ec-ai.mail.protection.outlook.com
  registrar_ns: markmonitor.com
  spf: true
  spf_record: v=spf1 include:_spf.salesforce.com include:spf.protection.outlook.com include:43881181.spf10.hubspotemail.net -all
hosts:
- a_record: 198.12.144.169
  a_record_owner: GoDaddy (secureserver.net) anycast forwarding address — not a live web origin
  host: ec.ai
  https: false
  https_note: 'Port 443 refuses the TLS handshake (SSLv3 alert handshake failure, alert 40) with every protocol, cipher and group combination tried, from three independent networks. Port 80 answers HTTP/1.1 409 Conflict from a Cloudflare edge with body "error code: 1001" (origin DNS resolution failure). No certificate could be retrieved, so no HSTS or expiry data exists to record.'
- host: cora.ec.ai
  https: false
  https_note: Resolves to 34.96.64.53 (Google Cloud LB). The certificate presented for SNI cora.ec.ai is CN=ragflow.devgcp.fiddler.ai, issued by Google Trust Services WR3 — a third party's host. Name mismatch; every request then answers HTTP 401 from Google Cloud Identity-Aware Proxy. Dangling DNS record.
- host: cogent.ec.ai
  https: false
  https_note: Resolves to 34.117.199.168 (Google Cloud LB). The certificate presented for SNI cogent.ec.ai is CN=*.race.co.jp, issued by Sectigo — an unrelated third party. Name mismatch; with verification disabled every path returns an ~886 KB HTML page belonging to that other site. Dangling DNS record.
kind: domain-security
layout: security
method: probed
name: Elemental Cognition Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elemental Cognition, probed live across 3 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Elemental Cognition
provider_slug: elemental-cognition
slug: elemental-cognition-domain-security
source_filename: elemental-cognition-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ec.ai\n  https: false\n  https_note: >-\n    Port 443 refuses the TLS handshake (SSLv3 alert handshake failure, alert 40) with every protocol,\n    cipher and group combination tried, from three independent networks. Port 80 answers HTTP/1.1\n    409 Conflict from a Cloudflare edge with body \"error code: 1001\" (origin DNS resolution failure).\n    No certificate could be retrieved, so no HSTS or expiry data exists to record.\n  a_record: 198.12.144.169\n  a_record_owner: GoDaddy (secureserver.net) anycast forwarding address — not a live web origin\n- host: cora.ec.ai\n  https: false\n  https_note: >-\n    Resolves to 34.96.64.53 (Google Cloud LB). The certificate presented for SNI cora.ec.ai is\n    CN=ragflow.devgcp.fiddler.ai, issued by Google Trust Services WR3 — a third party's host. Name\n    mismatch; every request then answers HTTP 401 from Google\
  \ Cloud Identity-Aware Proxy. Dangling\n    DNS record.\n- host: cogent.ec.ai\n  https: false\n  https_note: >-\n    Resolves to 34.117.199.168 (Google Cloud LB). The certificate presented for SNI cogent.ec.ai is\n    CN=*.race.co.jp, issued by Sectigo — an unrelated third party. Name mismatch; with verification\n    disabled every path returns an ~886 KB HTML page belonging to that other site. Dangling DNS\n    record.\ndomains:\n- domain: ec.ai\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: >-\n    v=spf1 include:_spf.salesforce.com include:spf.protection.outlook.com\n    include:43881181.spf10.hubspotemail.net -all\n  dmarc: true\n  dmarc_policy: quarantine\n  mx: ec-ai.mail.protection.outlook.com\n  registrar_ns: markmonitor.com\nfindings:\n- id: no-serving-tls\n  severity: high\n  detail: >-\n    The apex domain ec.ai terminates no usable TLS session and its HTTP origin is unresolvable at\n    the Cloudflare edge. Corporate mail (Microsoft 365) and SPF/DMARC remain configured,\
  \ so the\n    domain is still administered — the web presence specifically is gone.\n- id: dangling-subdomain-dns\n  severity: high\n  detail: >-\n    cogent.ec.ai and cora.ec.ai both point at Google Cloud load balancers that now serve\n    certificates for unrelated third parties (*.race.co.jp and ragflow.devgcp.fiddler.ai). Records\n    that outlive their backend on a shared cloud load balancer are the classic subdomain-takeover\n    precondition; these should be removed from DNS.\n- id: no-caa\n  severity: low\n  detail: No CAA record is published for ec.ai, so any public CA may issue for the domain.\n- id: no-dnssec\n  severity: low\n  detail: ec.ai is not DNSSEC signed.\nx-evidence:\n  checked: '2026-08-12'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elemental-cognition/refs/heads/main/security/elemental-cognition-domain-security.yml
summary_line: DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Natural Language Processing
- Reasoning
- Enterprise AI
- Knowledge Models
- Decision Support
---
