---
description: ''
domains:
- caa: []
  created: '1997-06-03'
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vastera.com
  expires: '2027-06-02'
  mx:
  - us-smtp-inbound-1.mimecast.com
  - us-smtp-inbound-2.mimecast.com
  nameservers:
  - albert.ns.cloudflare.com
  - eloise.ns.cloudflare.com
  registrar: Amazon Registrar, Inc.
  spf: true
  spf_record: v=spf1 mx include:spf.protection.outlook.com include:us._netblocks.mimecast.com -all
hosts:
- detail: no A record; curl HTTPS returned no response (000)
  host: vastera.com
  https: false
  reachable: false
- detail: no A record; curl HTTPS returned no response (000)
  host: www.vastera.com
  https: false
  reachable: false
kind: domain-security
layout: security
method: probed
name: Vastera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vastera, probed live across 2 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vastera
provider_slug: vastera
slug: vastera-domain-security
source_filename: vastera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: manual dig/curl/whois probes of vastera.com (no Website/baseURL in apis.yml; historical corporate domain)\nnote: Vastera, Inc. was acquired by JPMorgan Chase Bank, N.A. effective 2005-04-01 and no\n  longer operates a public website. The vastera.com domain (registered 1997-06-03) remains\n  actively held and is configured for email only — no A records resolve for the apex or www\n  hosts, so HTTPS/TLS/HSTS could not be evaluated.\nhosts:\n  - host: vastera.com\n    https: false\n    reachable: false\n    detail: no A record; curl HTTPS returned no response (000)\n  - host: www.vastera.com\n    https: false\n    reachable: false\n    detail: no A record; curl HTTPS returned no response (000)\ndomains:\n  - domain: vastera.com\n    dnssec: false\n    caa: []\n    spf: true\n    spf_record: 'v=spf1 mx include:spf.protection.outlook.com include:us._netblocks.mimecast.com -all'\n    dmarc: true\n    dmarc_policy: quarantine\n    mx:\n\
  \      - us-smtp-inbound-1.mimecast.com\n      - us-smtp-inbound-2.mimecast.com\n    nameservers:\n      - albert.ns.cloudflare.com\n      - eloise.ns.cloudflare.com\n    registrar: Amazon Registrar, Inc.\n    created: '1997-06-03'\n    expires: '2027-06-02'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vastera/refs/heads/main/security/vastera-domain-security.yml
summary_line: DMARC
tags:
- Company
- Global Trade Management
- Supply Chain
- Trade Compliance
- Logistics
- Acquired
---
