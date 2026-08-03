---
api_specs:
- filename: zotgpt-api-openapi.yml
  format: yaml
  label: ZotGPT API (Deprecated)
  slug: api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zotgpt/refs/heads/main/openapi/zotgpt-api-openapi.yml
- filename: zotgpt-gateway-openapi.yml
  format: yaml
  label: ZotGPT (UC Irvine) ZotGPT Gateway
  slug: zotgpt-gateway-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zotgpt/refs/heads/main/openapi/zotgpt-gateway-openapi.yml
description: 'Live TLS, transport, DNS, and identity-plane probe of the ZotGPT hosts. The probe is the clearest single piece of evidence for the platform''s multi-cloud posture: every interactive product terminates on a UC Irvine-owned AWS Application Load Balancer in us-west-2 under the *.aws.uci.edu naming convention, with an Amazon-issued certificate, while the developer API control plane terminates on Azure API Management in the same region. Two clouds, one campus namespace.'
domains: []
hosts:
- cloud: AWS
  host: zotgpt.uci.edu
  notes: Marketing and documentation site. Certificate CN is the AWS account's internal LB name, which is why the campus AWS account naming (zot-gpt-prod) is externally visible.
  protocol: HTTP/2
  resolves_to:
  - zotgpt-lb.zot-gpt-prod.aws.uci.edu
  - zotgpt-alb-prod-1683233264.us-west-2.elb.amazonaws.com
  - 44.237.46.108
  - 44.227.122.188
  server: nginx
  status: 200
  tls:
    issuer: C=US, O=Amazon, CN=Amazon RSA 2048 M04
    not_after: '2027-03-15'
    not_before: '2026-02-14'
    subject: CN=zotgpt-lb.zot-gpt-prod.aws.uci.edu
- auth_redirect: https://shib.service.uci.edu/idp/profile/SAML2/Redirect/SSO
  aws_account_env: zot-gpt-prod
  cloud: AWS
  host: chat.zotgpt.uci.edu
  notes: Redirects unauthenticated callers into the campus Shibboleth IdP. Sets secure, HttpOnly, SameSite=None OpenSAML session cookies.
  resolves_to:
  - zotgpt-lb.zot-gpt-prod.aws.uci.edu
  - zotgpt-alb-prod-1683233264.us-west-2.elb.amazonaws.com
  status: 302
- aws_account_env: oit-instructorbot-prod
  cloud: AWS
  host: classchat.zotgpt.uci.edu
  notes: Separate ALB and separate environment from Chat — the "modular architecture ... isolates each instance with separate policies" that UCI describes for classroom versus private use is visible in DNS.
  resolves_to:
  - oit-instrbt-lb.oit-instructorbot-prod.aws.uci.edu
  - oit-instrbt-alb-prod-679918224.us-west-2.elb.amazonaws.com
- aws_account_env: oit-zotgptcreator-prod
  cloud: AWS
  host: creator.zotgpt.uci.edu
  notes: A third isolated production environment.
  resolves_to:
  - oit-creator-lb.oit-zotgptcreator-prod.aws.uci.edu
  - oit-creator-alb-prod-1057247275.us-west-2.elb.amazonaws.com
- cloud: Azure
  host: portal.azureapi.zotgpt.uci.edu
  notes: Azure API Management developer portal, West US 2, fronted by Azure Traffic Manager. The APIM gateway itself (oit-apim-usw2.azure-api.net) answers with an APIM JSON envelope. This is the developer control plane for the deprecated API.
  resolves_to:
  - oit-apim-usw2.azure-api.net
  - apimgmttmljklbukrkr823ui1xipvjxn6zcs2mi4dh7zzcjwze.trafficmanager.net
  - oit-apim-usw2-westus2-01.regional.azure-api.net
  - 172.179.148.210
  status: 200
  title: UC Irvine API Management
- host: api.zotgpt.uci.edu
  notes: Documented data-plane host for the deprecated API. NXDOMAIN from the public internet — campus-internal or already withdrawn.
  resolves: false
  status: 0
- host: api.azureapi.zotgpt.uci.edu
  notes: Old base URL quoted in the migration guide. NXDOMAIN publicly.
  resolves: false
  status: 0
kind: domain-security
layout: security
method: probed
name: Zotgpt Domain Security
name_suffix: Domain Security
overview: Domain security posture for ZotGPT (UC Irvine), probed live across 7 host(s) and 0 registrable domain(s).
provider_name: ZotGPT (UC Irvine)
provider_slug: zotgpt
slug: zotgpt-domain-security
source_filename: zotgpt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: probed\nprovider: ZotGPT (UC Irvine)\nproviderId: zotgpt\ndescription: >-\n  Live TLS, transport, DNS, and identity-plane probe of the ZotGPT hosts. The\n  probe is the clearest single piece of evidence for the platform's multi-cloud\n  posture: every interactive product terminates on a UC Irvine-owned AWS\n  Application Load Balancer in us-west-2 under the *.aws.uci.edu naming\n  convention, with an Amazon-issued certificate, while the developer API control\n  plane terminates on Azure API Management in the same region. Two clouds, one\n  campus namespace.\ntags:\n  - Domain Security\n  - TLS\n  - Multi-Cloud\n  - Shibboleth\nhosts:\n  - host: zotgpt.uci.edu\n    status: 200\n    protocol: HTTP/2\n    server: nginx\n    cloud: AWS\n    resolves_to:\n      - zotgpt-lb.zot-gpt-prod.aws.uci.edu\n      - zotgpt-alb-prod-1683233264.us-west-2.elb.amazonaws.com\n      - 44.237.46.108\n      - 44.227.122.188\n    tls:\n      issuer: 'C=US, O=Amazon,\
  \ CN=Amazon RSA 2048 M04'\n      subject: 'CN=zotgpt-lb.zot-gpt-prod.aws.uci.edu'\n      not_before: '2026-02-14'\n      not_after: '2027-03-15'\n    notes: >-\n      Marketing and documentation site. Certificate CN is the AWS account's\n      internal LB name, which is why the campus AWS account naming\n      (zot-gpt-prod) is externally visible.\n  - host: chat.zotgpt.uci.edu\n    status: 302\n    cloud: AWS\n    aws_account_env: zot-gpt-prod\n    resolves_to:\n      - zotgpt-lb.zot-gpt-prod.aws.uci.edu\n      - zotgpt-alb-prod-1683233264.us-west-2.elb.amazonaws.com\n    auth_redirect: https://shib.service.uci.edu/idp/profile/SAML2/Redirect/SSO\n    notes: >-\n      Redirects unauthenticated callers into the campus Shibboleth IdP. Sets\n      secure, HttpOnly, SameSite=None OpenSAML session cookies.\n  - host: classchat.zotgpt.uci.edu\n    cloud: AWS\n    aws_account_env: oit-instructorbot-prod\n    resolves_to:\n      - oit-instrbt-lb.oit-instructorbot-prod.aws.uci.edu\n      - oit-instrbt-alb-prod-679918224.us-west-2.elb.amazonaws.com\n\
  \    notes: >-\n      Separate ALB and separate environment from Chat — the \"modular\n      architecture ... isolates each instance with separate policies\" that UCI\n      describes for classroom versus private use is visible in DNS.\n  - host: creator.zotgpt.uci.edu\n    cloud: AWS\n    aws_account_env: oit-zotgptcreator-prod\n    resolves_to:\n      - oit-creator-lb.oit-zotgptcreator-prod.aws.uci.edu\n      - oit-creator-alb-prod-1057247275.us-west-2.elb.amazonaws.com\n    notes: A third isolated production environment.\n  - host: portal.azureapi.zotgpt.uci.edu\n    status: 200\n    cloud: Azure\n    resolves_to:\n      - oit-apim-usw2.azure-api.net\n      - apimgmttmljklbukrkr823ui1xipvjxn6zcs2mi4dh7zzcjwze.trafficmanager.net\n      - oit-apim-usw2-westus2-01.regional.azure-api.net\n      - 172.179.148.210\n    title: 'UC Irvine API Management'\n    notes: >-\n      Azure API Management developer portal, West US 2, fronted by Azure Traffic\n      Manager. The APIM gateway itself (oit-apim-usw2.azure-api.net)\
  \ answers with\n      an APIM JSON envelope. This is the developer control plane for the\n      deprecated API.\n  - host: api.zotgpt.uci.edu\n    status: 0\n    resolves: false\n    notes: >-\n      Documented data-plane host for the deprecated API. NXDOMAIN from the public\n      internet — campus-internal or already withdrawn.\n  - host: api.azureapi.zotgpt.uci.edu\n    status: 0\n    resolves: false\n    notes: Old base URL quoted in the migration guide. NXDOMAIN publicly.\nidentity_plane:\n  idp: https://shib.service.uci.edu/idp/profile/SAML2/Redirect/SSO\n  metadata: https://shib.service.uci.edu/idp/shibboleth\n  metadata_status: 200\n  metadata_content_type: application/xml\n  protocol: SAML 2.0 (Shibboleth)\n  notes: >-\n    The IdP publishes its SAML metadata anonymously — the only machine-readable\n    descriptor anywhere in the ZotGPT estate that a third party can retrieve\n    without credentials.\nemail_domain_security:\n  domain: uci.edu\n  spf: 'v=spf1 include:%{ir}.%{v}.%{d}.spf.has.pphosted.com\
  \ ?all'\n  spf_notes: >-\n    Proofpoint macro-expanded include with a soft ?all rather than -all.\n  dmarc: 'v=DMARC1; p=none; fo=1; rua=mailto:dmarc_rua@emaildefense.proofpoint.com; ruf=mailto:dmarc_ruf@emaildefense.proofpoint.com'\n  dmarc_policy: none\n  dmarc_notes: Monitoring only; no quarantine or reject enforcement.\n  dnssec: not enabled (no DS record for uci.edu)\n  caa: no CAA record published for uci.edu\nfindings:\n  - severity: informational\n    finding: >-\n      Multi-cloud is real and externally verifiable — AWS us-west-2 for every\n      application plane, Azure West US 2 for the API management plane.\n  - severity: informational\n    finding: >-\n      Product isolation is real — Chat, ClassChat, and Creator each run in their\n      own named AWS production environment behind their own load balancer.\n  - severity: low\n    finding: >-\n      No security.txt at /.well-known/security.txt on any ZotGPT host (404).\n  - severity: low\n    finding: >-\n      No robots.txt\
  \ on zotgpt.uci.edu (404), and no sitemap.xml.\n  - severity: low\n    finding: >-\n      uci.edu publishes no CAA record and no DS record (DNSSEC not enabled), and\n      DMARC is at p=none.\n  - severity: informational\n    finding: >-\n      Internal AWS account and environment names (zot-gpt-prod,\n      oit-instructorbot-prod, oit-zotgptcreator-prod) are disclosed through\n      certificate subjects and CNAME chains.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zotgpt/refs/heads/main/security/zotgpt-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Domain Security
- TLS
- Multi-Cloud
- Shibboleth
---
