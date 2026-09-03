---
api_key_in: []
api_specs:
- filename: university-of-gothenburg-korp-api-openapi.yml
  format: yaml
  label: Korp API v8 — Corpus Concordance Search
  slug: korp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-gothenburg/refs/heads/main/openapi/university-of-gothenburg-korp-api-openapi.yml
- filename: university-of-gothenburg-metadata-api-openapi.yml
  format: yaml
  label: Språkbanken Text Metadata API v3
  slug: sbx-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-gothenburg/refs/heads/main/openapi/university-of-gothenburg-metadata-api-openapi.yml
- filename: university-of-gothenburg-mink-api-openapi.yml
  format: yaml
  label: Mink API v3 — Bring Your Own Corpus
  slug: mink-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-gothenburg/refs/heads/main/openapi/university-of-gothenburg-mink-api-openapi.yml
- filename: university-of-gothenburg-sparv-api-openapi.yml
  format: yaml
  label: Sparv API v3 — Text Annotation Pipeline
  slug: sparv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-gothenburg/refs/heads/main/openapi/university-of-gothenburg-sparv-api-openapi.yml
- filename: university-of-gothenburg-karp-api-openapi.yml
  format: yaml
  label: Karp API v7 — Lexical Resource Editing
  slug: karp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-gothenburg/refs/heads/main/openapi/university-of-gothenburg-karp-api-openapi.yml
- filename: university-of-gothenburg-karp-search-api-openapi.yml
  format: yaml
  label: Karp Search API v1 — Karps sökgränssnitt
  slug: karp-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-gothenburg/refs/heads/main/openapi/university-of-gothenburg-karp-search-api-openapi.yml
- filename: university-of-gothenburg-gupea-oai-pmh-openapi.yml
  format: yaml
  label: GUPEA Repository OAI-PMH 2.0 Interface
  slug: gupea-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-gothenburg/refs/heads/main/openapi/university-of-gothenburg-gupea-oai-pmh-openapi.yml
auth_types: []
description: 'Authentication posture per surface, split by operator. The finding worth stating plainly: every public read surface the University of Gothenburg operates answered an ANONYMOUS request with HTTP 200. There is no API key to obtain, no registration flow, no developer account and no published rate limit anywhere in this profile. Authorisation exists in exactly one place — Mink, where writing your own corpus requires a token — and that login rides on the same SWAMID/eduGAIN federation the institution operates its own IdP inside of.'
kind: authentication
layout: security
method: probed
name: University Of Gothenburg Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Gothenburg declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: University of Gothenburg
provider_slug: university-of-gothenburg
scheme_count: 0
schemes: []
slug: university-of-gothenburg-authentication
source_filename: university-of-gothenburg-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "# x-method: derived\n# x-source-url: https://ws.spraakbanken.gu.se/docs/\n# Written by API Evangelist for the api-evangelist/university-of-gothenburg repo on\n# 2026-09-01. `x-method` uses the provenance-manifest vocabulary; the artifact's own\n# `method:` key uses the enrichment-contract vocabulary. They are not in conflict.\ngenerated: '2026-09-01'\nmethod: probed\nsource: >-\n  Anonymous live requests on 2026-09-01 against every surface listed below, plus the\n  securitySchemes declared in each of the six Språkbanken Text OpenAPI documents stored under\n  openapi/_original/.\ndescription: >-\n  Authentication posture per surface, split by operator. The finding worth stating plainly:\n  every public read surface the University of Gothenburg operates answered an ANONYMOUS request\n  with HTTP 200. There is no API key to obtain, no registration flow, no developer account and\n  no published rate limit anywhere in this profile. Authorisation exists in exactly one place —\n \
  \ Mink, where writing your own corpus requires a token — and that login rides on the same\n  SWAMID/eduGAIN federation the institution operates its own IdP inside of.\nsurfaces:\n  - name: Korp API v8\n    url: https://ws.spraakbanken.gu.se/ws/korp/v8\n    x-operator: institution\n    type: none\n    verified: '2026-09-01'\n    detail: >-\n      Anonymous GET /info returned HTTP 200 application/json, 25,974 bytes, listing 1,133 corpora.\n      The specification declares a `basicAuth` HTTP Basic scheme applied globally, but it gates\n      access to PROTECTED corpora only: unauthenticated callers get the open corpora and the full\n      query, count, statistics and word-picture command set. No sign-up is published for the\n      protected tier.\n  - name: Språkbanken Text Metadata API v3\n    url: https://ws.spraakbanken.gu.se/ws/metadata/v3\n    x-operator: institution\n    type: none\n    verified: '2026-09-01'\n    detail: >-\n      No securitySchemes declared at all. Anonymous GET /\
  \ returned HTTP 200 with 2,531,491 bytes\n      of catalogue JSON; GET /list-ids returned 200 with 1,499 resource ids. Fully open read.\n  - name: Karp API v7 (editing mode)\n    url: https://spraakbanken4.it.gu.se/karp/v7\n    x-operator: institution\n    type: bearer + api-key (declared, not required for read)\n    verified: '2026-09-01'\n    detail: >-\n      Declares `APIKeyQuery` and `HTTPBearer` securitySchemes. Anonymous GET /resources/ returned\n      HTTP 200 with 1,042,817 bytes, so the read surface is open; the declared schemes gate the\n      write and history operations. No key-issuance flow is published.\n  - name: Karp search API v1 (Karps sökgränssnitt)\n    url: https://spraakbanken4.it.gu.se/karps/v1\n    x-operator: institution\n    type: none\n    verified: '2026-09-01'\n    detail: >-\n      Declares `HTTPBearer` and `APIKeyHeader` but applies neither to the three published\n      operations. Anonymous GET /config returned HTTP 200 with 47,203 bytes describing 31\n\
  \      lexical resources.\n  - name: Sparv API v3\n    url: https://ws.spraakbanken.gu.se/ws/sparv/v3\n    x-operator: institution\n    type: api-key (declared, not required for status operations)\n    verified: '2026-09-01'\n    detail: >-\n      Declares an `ApiKeyAuth` scheme. Anonymous GET /ping returned HTTP 200\n      {\"message\": \"PONG\", \"time\": 0.0041}, and GET / returned 200 with a structured\n      {\"error\": {\"message\": \"No input was found.\"}} rather than a 401 — so the service answers\n      unauthenticated callers and rejects on input, not on identity, for the status surface.\n  - name: Mink API v3\n    url: https://ws.spraakbanken.gu.se/ws/mink/v3\n    x-operator: institution\n    type: oauth2 bearer + api-key header\n    verified: '2026-09-01'\n    detail: >-\n      The only surface in this profile with a real authorisation model. Declares\n      `OAuth2PasswordBearer` and `APIKeyHeader`. Anonymous GET /info returned HTTP 200 with the\n      job status-code catalogue,\
  \ so the informational surface is open, while the 63-path corpus\n      create/upload/run/publish surface is token-gated. Mink's user accounts are federated\n      logins, which is why the institution's own SWAMID IdP (below) is load-bearing for this API\n      rather than incidental to it.\n  - name: GUPEA DSpace 8 REST API\n    url: https://gupea.ub.gu.se/server/api\n    x-operator: institution\n    type: none for read; token for write\n    verified: '2026-09-01'\n    detail: >-\n      Anonymous GET returned HTTP 200 application/hal+json, 8,531 bytes, with\n      \"dspaceName\": \"GUPEA\", \"dspaceVersion\": \"DSpace 8.3-SNAPSHOT\" and an `authn` link in\n      `_links`. Stock DSpace: anonymous read of public items, JWT for write. The DSpace REST\n      contract is the DSpace project's, not the University's, and is deliberately NOT stored\n      under this slug — only the deployment is recorded.\n  - name: GUPEA OAI-PMH 2.0\n    url: https://gupea.ub.gu.se/server/oai/request\n    x-operator:\
  \ institution\n    type: none\n    verified: '2026-09-01'\n    detail: Anonymous. OAI-PMH has no authentication layer by design.\n  - name: Shibboleth Identity Provider (SWAMID / eduGAIN)\n    url: https://idp3.it.gu.se/idp/shibboleth\n    x-operator: federation\n    type: saml2\n    verified: '2026-09-01'\n    detail: >-\n      The University's own Shibboleth SAML 2.0 IdP, scope `gu.se`, published as signed metadata\n      through the SWAMID MDQ service (HTTP 200 application/samlmetadata+xml, 13,045 bytes). SSO\n      endpoints at /idp/profile/SAML2/POST/SSO and /idp/profile/SAML2/Redirect/SSO. This is not\n      an API the University sells; it is the identity surface everything else in Swedish higher\n      education authenticates against, and it is machine-readable.\n  - name: Microsoft AD FS identity provider\n    url: http://idp.auth.gu.se/adfs/services/trust\n    x-operator: federation\n    type: ws-trust / saml2\n    verified: '2026-09-01'\n    detail: >-\n      A second University\
  \ of Gothenburg entity in the SWAMID aggregate, DisplayName \"University\n      of Gothenburg (ADFS)\". Registered by the institution; the AD FS product is Microsoft's.\n      Recorded, not scored as a contract.\n  - name: Microsoft 365 / SharePoint staff portal\n    url: https://medarbetarportalen.gu.se/\n    x-operator: tenant\n    type: oauth2 (Microsoft Entra ID)\n    verified: '2026-09-01'\n    detail: >-\n      Redirects to login.microsoftonline.com with Entra tenant id\n      0798ed31-f5b0-4935-863c-73ee2505806e and resource gunet.sharepoint.com. A Microsoft tenancy\n      on a University hostname. Recorded as a relationship; no Microsoft contract is stored here.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-gothenburg/refs/heads/main/authentication/university-of-gothenburg-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Sweden
- Research
- Research Data
- Research Repository
- Open Data
- Library
- OAI-PMH
- Identity Federation
- Language Technology
- Natural Language Processing
- Corpus Linguistics
---
