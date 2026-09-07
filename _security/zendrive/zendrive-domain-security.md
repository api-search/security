---
description: 'Probed by hand rather than by probe-domain-security.py, which reported "no-hosts" because this record deliberately wires no Website pointer and no API baseURL — Zendrive has no live web host to point at. The DNS-layer posture is still measurable, and it is the most interesting finding in this profile: the zendrive.com zone is actively maintained even though nothing is served from it. A Google Trust Services certificate covering zendrive.com and *.zendrive.com was issued on 2026-08-26 (Cloudflare Universal SSL), DMARC is at p=reject with strict alignment and a live reporting mailbox, and CAA is a long, curated issuer allowlist with an iodef security contact. Someone is still holding and defending this domain; they have simply removed every A record.'
domains: []
hosts:
- dns:
    a_records: []
    caa:
      iodef: mailto:security@zendrive.com
      issue:
      - letsencrypt.org
      - pki.goog; cansignhttpexchanges=yes
      - ssl.com
      - amazon.com
      - comodoca.com
      - digicert.com; cansignhttpexchanges=yes
      issuewild:
      - comodoca.com
      - digicert.com; cansignhttpexchanges=yes
      - letsencrypt.org
      - pki.goog; cansignhttpexchanges=yes
      - ssl.com
      note: The iodef address is a CAA certificate-violation reporting contact (RFC 8659), NOT a vulnerability disclosure program. It is recorded as a security contact of record and nothing more; no Security or VulnerabilityDisclosure pointer is emitted from it.
      present: true
    dmarc:
      alignment: strict (adkim=s, aspf=s)
      pct: 100
      policy: reject
      present: true
      record: v=DMARC1; p=reject; rua=mailto:sec-ops@zendrive.com; pct=100; sp=reject; adkim=s; aspf=s
      rua: mailto:sec-ops@zendrive.com
      subdomain_policy: reject
    dnssec:
      dnskey: false
      ds: false
      enabled: false
    mx:
    - aspmx.l.google.com (10)
    - alt1.aspmx.l.google.com (20)
    - alt2.aspmx.l.google.com (20)
    - aspmx2.googlemail.com (30)
    - aspmx3.googlemail.com (30)
    mx_note: Google Workspace MX records are still published, so mail may still route.
    nameservers:
    - melany.ns.cloudflare.com
    - thaddeus.ns.cloudflare.com
    spf:
      note: No TXT records at all on the apex, so no SPF policy is published.
      present: false
  host: zendrive.com
  https:
    note: No A/AAAA record. Connection cannot be established, so TLS and HSTS are unmeasurable at this host.
    reachable: false
- dns:
    a_records:
    - 172.67.161.199
    - 104.21.9.243
    provider: Cloudflare
  host: docs.zendrive.com
  https:
    hsts: false
    note: 'Answers, but only with Cloudflare''s dangling-CNAME error ("error code: 1014", 17 bytes, text/plain). No HSTS header is returned on that error response.'
    reachable: true
    status: 403
  tls:
    certificate_issuer: C=US, O=Google Trust Services, CN=WE1
    certificate_subject: CN=zendrive.com
    not_after: '2026-11-24'
    not_before: '2026-08-26'
    note: A currently valid certificate, issued well after the company wound down its developer program — consistent with Cloudflare Universal SSL renewing automatically for a zone that is still on the account.
    subject_alt_names:
    - zendrive.com
    - '*.zendrive.com'
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Zendrive Domain Security
name_suffix: Domain Security
overview: Domain security posture for Zendrive, probed live across 2 host(s) and 0 registrable domain(s). 2 host(s) serve HTTPS; 0 advertise HSTS.
provider_name: Zendrive
provider_slug: zendrive
slug: zendrive-domain-security
source_filename: zendrive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: dns + tls probe of zendrive.com and docs.zendrive.com\nname: Zendrive domain security posture\ndescription: >-\n  Probed by hand rather than by probe-domain-security.py, which reported \"no-hosts\" because\n  this record deliberately wires no Website pointer and no API baseURL — Zendrive has no live\n  web host to point at. The DNS-layer posture is still measurable, and it is the most\n  interesting finding in this profile: the zendrive.com zone is actively maintained even\n  though nothing is served from it. A Google Trust Services certificate covering zendrive.com\n  and *.zendrive.com was issued on 2026-08-26 (Cloudflare Universal SSL), DMARC is at\n  p=reject with strict alignment and a live reporting mailbox, and CAA is a long, curated\n  issuer allowlist with an iodef security contact. Someone is still holding and defending this\n  domain; they have simply removed every A record.\nhosts:\n- host: zendrive.com\n  https:\n\
  \    reachable: false\n    note: No A/AAAA record. Connection cannot be established, so TLS and HSTS are unmeasurable at this host.\n  dns:\n    a_records: []\n    nameservers:\n    - melany.ns.cloudflare.com\n    - thaddeus.ns.cloudflare.com\n    mx:\n    - aspmx.l.google.com (10)\n    - alt1.aspmx.l.google.com (20)\n    - alt2.aspmx.l.google.com (20)\n    - aspmx2.googlemail.com (30)\n    - aspmx3.googlemail.com (30)\n    mx_note: Google Workspace MX records are still published, so mail may still route.\n    dnssec:\n      dnskey: false\n      ds: false\n      enabled: false\n    caa:\n      present: true\n      issue:\n      - letsencrypt.org\n      - 'pki.goog; cansignhttpexchanges=yes'\n      - ssl.com\n      - amazon.com\n      - comodoca.com\n      - 'digicert.com; cansignhttpexchanges=yes'\n      issuewild:\n      - comodoca.com\n      - 'digicert.com; cansignhttpexchanges=yes'\n      - letsencrypt.org\n      - 'pki.goog; cansignhttpexchanges=yes'\n      - ssl.com\n      iodef:\
  \ mailto:security@zendrive.com\n      note: >-\n        The iodef address is a CAA certificate-violation reporting contact (RFC 8659), NOT a\n        vulnerability disclosure program. It is recorded as a security contact of record and\n        nothing more; no Security or VulnerabilityDisclosure pointer is emitted from it.\n    spf:\n      present: false\n      note: No TXT records at all on the apex, so no SPF policy is published.\n    dmarc:\n      present: true\n      record: 'v=DMARC1; p=reject; rua=mailto:sec-ops@zendrive.com; pct=100; sp=reject; adkim=s; aspf=s'\n      policy: reject\n      subdomain_policy: reject\n      pct: 100\n      alignment: strict (adkim=s, aspf=s)\n      rua: mailto:sec-ops@zendrive.com\n- host: docs.zendrive.com\n  https:\n    reachable: true\n    status: 403\n    note: >-\n      Answers, but only with Cloudflare's dangling-CNAME error (\"error code: 1014\", 17 bytes,\n      text/plain). No HSTS header is returned on that error response.\n    hsts: false\n\
  \  tls:\n    certificate_subject: CN=zendrive.com\n    certificate_issuer: 'C=US, O=Google Trust Services, CN=WE1'\n    not_before: '2026-08-26'\n    not_after: '2026-11-24'\n    subject_alt_names:\n    - zendrive.com\n    - '*.zendrive.com'\n    note: >-\n      A currently valid certificate, issued well after the company wound down its developer\n      program — consistent with Cloudflare Universal SSL renewing automatically for a zone\n      that is still on the account.\n  dns:\n    a_records:\n    - 172.67.161.199\n    - 104.21.9.243\n    provider: Cloudflare\nfindings:\n- Domain is retained and actively certificated, but serves nothing.\n- DNSSEC is not enabled.\n- DMARC is strong (p=reject, sp=reject, strict alignment); SPF is absent, which is a real gap.\n- CAA is present and unusually thorough, with an iodef security contact.\n- No HSTS can be observed anywhere, because no host serves a successful response.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zendrive/refs/heads/main/security/zendrive-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Telematics
- Mobility
- Insurance
- Automotive
- Fleet Management
- Driving Behavior
- Mobile SDK
- Risk
- Acquired
---
