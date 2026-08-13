---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: elementus.io
  spf: true
hosts:
- failure: dns-nxdomain
  host: www.elementus.io
  https: false
- cname: atapi-alb-370503343.us-east-1.elb.amazonaws.com
  failure: dangling-cname
  host: attribution-api.elementus.io
  https: false
kind: domain-security
layout: security
method: probed
name: Elementus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elementus, probed live across 2 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Elementus
provider_slug: elementus
slug: elementus-domain-security
source_filename: elementus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.elementus.io\n  https: false\n  failure: dns-nxdomain\n- host: attribution-api.elementus.io\n  https: false\n  failure: dangling-cname\n  cname: atapi-alb-370503343.us-east-1.elb.amazonaws.com\ndomains:\n- domain: elementus.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n\n# --- Added by the enrichment pass, same probe date, same method. ---\n# The base probe records \"https: false\" for both hosts. The reason matters more\n# than the flag: this is not a TLS failure, it is an absent origin.\n\ndns_posture:\n  zone_live: true\n  nameservers:\n  - carmelo.ns.cloudflare.com\n  - magali.ns.cloudflare.com\n  mx_live: true\n  mx:\n  - aspmx.l.google.com\n  - alt1.aspmx.l.google.com\n  - alt2.aspmx.l.google.com\n  - alt3.aspmx.l.google.com\n  - alt4.aspmx.l.google.com\n  note: >-\n    The elementus.io zone is intact and still\
  \ routes mail to Google Workspace,\n    but every web and API hostname under it is either missing or points at\n    infrastructure that no longer exists.\n\nfindings:\n- id: apex-no-address-record\n  severity: informational\n  host: elementus.io\n  observed: 'NOERROR with no A, AAAA or CNAME answer'\n  detail: >-\n    The apex resolves in the sense that the zone answers, but it publishes no\n    address record, so the marketing site cannot be reached.\n  checked: '2026-08-12'\n\n- id: www-nxdomain\n  severity: informational\n  host: www.elementus.io\n  observed: NXDOMAIN\n  detail: >-\n    The primary marketing hostname has been removed from DNS. The Internet\n    Archive holds a 200 capture of it as recently as 2026-06-23; crawling of the\n    domain stops entirely after 2026-06-30.\n  checked: '2026-08-12'\n\n- id: dangling-cname-attribution-api\n  severity: medium\n  host: attribution-api.elementus.io\n  observed: 'CNAME -> atapi-alb-370503343.us-east-1.elb.amazonaws.com (NXDOMAIN)'\n\
  \  detail: >-\n    The production API hostname still publishes a CNAME to an AWS Application\n    Load Balancer that no longer exists. A dangling CNAME to a deprovisioned\n    AWS resource is a subdomain-takeover precondition: whoever next allocates a\n    load balancer able to answer for that name inherits the hostname.\n  remediation: >-\n    Remove the CNAME, or re-point it at infrastructure Elementus operates.\n  checked: '2026-08-12'\n\n- id: dangling-cname-app\n  severity: medium\n  host: app.elementus.io\n  observed: 'CNAME -> d31epqv6t9q4s6.cloudfront.net (NOERROR, no address)'\n  detail: >-\n    The application hostname points at a CloudFront distribution that is\n    disabled or deleted. Same takeover precondition as the API host.\n  remediation: >-\n    Remove the CNAME, or re-point it at a distribution Elementus operates.\n  checked: '2026-08-12'\n\n- id: staging-host-third-party-controlled\n  severity: high\n  host: api-staging.elementus.io\n  observed: 'CNAME -> ec2-34-231-243-167.compute-1.amazonaws.com\
  \ (34.231.243.167); TCP connect times out'\n  detail: >-\n    THIRD-PARTY REPORT, NOT A LIVE OBSERVATION BY API EVANGELIST. The Internet\n    Archive's only capture of this hostname, taken 2026-05-30, is not an\n    Elementus page: it is a static page titled \"Subdomain Takeover — Proof of\n    Concept\" stating that the hostname resolved to a host controlled by a\n    self-identified security researcher, naming finding ID vbeta-c6lvZ-9z and\n    the contact address security@pentestsec.com. API Evangelist did not verify\n    the claim, did not contact the reporter, and takes no position on whether it\n    is genuine. What API Evangelist itself observed on 2026-08-12 is only this:\n    the hostname still publishes a CNAME to an EC2 instance hostname, and that\n    address accepts no connection on port 80 or 443.\n  evidence:\n  - url: http://web.archive.org/web/20260530064751/http://api-staging.elementus.io/\n    status: 200\n    note: archived third-party page, not served by Elementus\
  \ infrastructure today\n  - url: https://api-staging.elementus.io/\n    status: 0\n    note: 'curl exit 28, connection timed out after 8s (2026-08-12)'\n  remediation: >-\n    Remove the dangling record for api-staging.elementus.io, or re-point it at a\n    host Elementus operates.\n  checked: '2026-08-12'\n\nsummary: >-\n  SPF and DMARC are published (DMARC p=none, monitor-only). DNSSEC is not\n  enabled and no CAA record is published, so certificate issuance for\n  elementus.io is unconstrained — which compounds the three dangling hostnames\n  above, since an attacker who claims one can also obtain a certificate for it.\n  No TLS or HSTS posture could be measured on any host because no host answered.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elementus/refs/heads/main/security/elementus-domain-security.yml
summary_line: DMARC
tags:
- Company
- Blockchain
- Cryptocurrency
- Analytics
- Compliance
- Financial Crime
- Sanctions Screening
- Data
- Web3
---
