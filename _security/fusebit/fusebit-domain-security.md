---
api_specs:
- filename: fusebit-http-api-core-openapi.yml
  format: yaml
  label: Fusebit HTTP API
  slug: apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fusebit/refs/heads/main/openapi/fusebit-http-api-core-openapi.yml
description: ''
domains:
- a_record: false
  caa: []
  caa_note: No CAA record — nothing constrains which CA may issue for this domain.
  created: '2019-04-10'
  dmarc: false
  dmarc_note: No record at _dmarc.fusebit.io. With no DMARC policy and a soft-fail SPF, a receiver has no instruction to reject spoofed mail from this domain.
  dnssec: false
  dnssec_evidence: no DNSKEY and no DS record returned (dig DNSKEY/DS fusebit.io @1.1.1.1)
  domain: fusebit.io
  expires: '2027-04-10'
  mx: true
  mx_note: Google Workspace mail routing is still live for a domain whose web presence is entirely gone.
  mx_records:
  - aspmx.l.google.com
  - alt1.aspmx.l.google.com
  - alt2.aspmx.l.google.com
  - aspmx2.googlemail.com
  - aspmx3.googlemail.com
  nameservers:
  - dns1.registrar-servers.com
  - dns2.registrar-servers.com
  registrar: NameCheap, Inc.
  spf: true
  spf_note: Soft-fail (~all) rather than hard-fail (-all). Still names Zoho Campaigns (zcsend.net) and Mailchimp (servers.mcsv.net) as authorized senders for a brand that no longer operates.
  spf_record: v=spf1 include:_spf.google.com include:zcsend.net include:servers.mcsv.net ~all
  txt_verifications:
  - MS=BCC655C596ADBD2570A850B3BFC55EDE7BFB2C68 (Microsoft)
  - google-site-verification x4
  updated: '2026-08-12'
  zone_published: true
hosts:
- a_record: null
  host: fusebit.io
  hsts: null
  https: false
  result: dns-nxdomain
  tls: null
- a_record: null
  host: www.fusebit.io
  https: false
  result: dns-nxdomain
- a_record: null
  host: developer.fusebit.io
  https: false
  result: dns-nxdomain
- a_record: null
  host: api.us-west-1.on.fusebit.io
  https: false
  note: The host named by servers[] in both published OpenAPI documents (region variable resolved to its declared default).
  result: dns-nxdomain
- a_record: null
  host: manage.fusebit.io
  https: false
  result: dns-nxdomain
- a_record: null
  host: cdn.fusebit.io
  https: false
  result: dns-nxdomain
hosts_probed: 6
kind: domain-security
layout: security
method: probed
name: Fusebit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fusebit, probed live across 6 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Fusebit
provider_slug: fusebit
slug: fusebit-domain-security
source_filename: fusebit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of every host in apis.yml and every OpenAPI servers[] host, 2026-09-10\nprovider: Fusebit\nproviderId: fusebit\nsummary: >-\n  The fusebit.io zone is still published and still routes MAIL, but it serves no web. Every host\n  fails to resolve an A record, so there is no TLS endpoint to assess and no HSTS header to read.\n  DNSSEC is not enabled, no CAA record constrains certificate issuance, and no DMARC policy protects\n  a domain whose MX still points at Google Workspace — an unusual residual risk on a retired brand:\n  mail for @fusebit.io is still deliverable and unauthenticated senders are not rejected.\nhosts:\n  - host: fusebit.io\n    a_record: null\n    https: false\n    result: dns-nxdomain\n    tls: null\n    hsts: null\n  - host: www.fusebit.io\n    a_record: null\n    https: false\n    result: dns-nxdomain\n  - host: developer.fusebit.io\n    a_record: null\n    https: false\n    result: dns-nxdomain\n\
  \  - host: api.us-west-1.on.fusebit.io\n    a_record: null\n    https: false\n    result: dns-nxdomain\n    note: The host named by servers[] in both published OpenAPI documents (region variable resolved to its declared default).\n  - host: manage.fusebit.io\n    a_record: null\n    https: false\n    result: dns-nxdomain\n  - host: cdn.fusebit.io\n    a_record: null\n    https: false\n    result: dns-nxdomain\ndomains:\n  - domain: fusebit.io\n    registrar: 'NameCheap, Inc.'\n    created: '2019-04-10'\n    expires: '2027-04-10'\n    updated: '2026-08-12'\n    nameservers: [dns1.registrar-servers.com, dns2.registrar-servers.com]\n    zone_published: true\n    a_record: false\n    dnssec: false\n    dnssec_evidence: 'no DNSKEY and no DS record returned (dig DNSKEY/DS fusebit.io @1.1.1.1)'\n    caa: []\n    caa_note: No CAA record — nothing constrains which CA may issue for this domain.\n    spf: true\n    spf_record: 'v=spf1 include:_spf.google.com include:zcsend.net include:servers.mcsv.net\
  \ ~all'\n    spf_note: >-\n      Soft-fail (~all) rather than hard-fail (-all). Still names Zoho Campaigns (zcsend.net) and\n      Mailchimp (servers.mcsv.net) as authorized senders for a brand that no longer operates.\n    dmarc: false\n    dmarc_note: >-\n      No record at _dmarc.fusebit.io. With no DMARC policy and a soft-fail SPF, a receiver has no\n      instruction to reject spoofed mail from this domain.\n    mx: true\n    mx_records: [aspmx.l.google.com, alt1.aspmx.l.google.com, alt2.aspmx.l.google.com, aspmx2.googlemail.com, aspmx3.googlemail.com]\n    mx_note: Google Workspace mail routing is still live for a domain whose web presence is entirely gone.\n    txt_verifications:\n      - 'MS=BCC655C596ADBD2570A850B3BFC55EDE7BFB2C68 (Microsoft)'\n      - 'google-site-verification x4'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fusebit/refs/heads/main/security/fusebit-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Developer Tools
- Embedded iPaaS
- Integration
- Serverless
- OAuth
- Acquired
---
