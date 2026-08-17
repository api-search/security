---
api_key_in: []
auth_types:
- http
description: 'Hashnode authenticates the GraphQL API with a single scheme: a long-lived Personal Access Token sent in the Authorization header. There is no OAuth, no OIDC, no scope model, and no mTLS - so there is no scopes/ artifact for this provider. Authorization is layered on top of authentication in two independent ways: a publication role model (OWNER / EDITOR / CONTRIBUTOR) and a subscription gate (the target publication must be on the Pro plan).'
kind: authentication
layout: security
method: searched
name: Hashnode Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hashnode secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hashnode
provider_slug: hashnode
scheme_count: 1
schemes:
- bearer_prefix_required: false
  format: opaque
  handling_rules:
  - Supply the token via the HASHNODE_PAT environment variable and interpolate it at request time.
  - Never inline the literal token into a command string, file, script, or commit.
  - Never ask a user to paste the token into a conversation and never print or log it.
  header: Authorization
  in: header
  issuance:
    expiry: none documented
    path: Account Settings -> Developer / API tokens -> Generate new token
    rotation: manual, from the dashboard
    url: https://hashnode.com/settings/developer
  name: PersonalAccessToken
  note: The "Bearer " prefix is optional and case-insensitive. A deactivated user's token is treated as unauthenticated.
  scheme: bearer
  scope_of_power: Full write access to every publication the user can act on - publish, edit, and delete. Hashnode's own guidance is to treat it as a password.
  type: http
slug: hashnode-authentication
source_filename: hashnode-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://raw.githubusercontent.com/Hashnode/gql-skill/main/skills/gql-api/references/auth-and-roles.md\ndocs: https://github.com/Hashnode/gql-skill/blob/main/skills/gql-api/references/auth-and-roles.md\ndescription: >-\n  Hashnode authenticates the GraphQL API with a single scheme: a long-lived\n  Personal Access Token sent in the Authorization header. There is no OAuth, no\n  OIDC, no scope model, and no mTLS - so there is no scopes/ artifact for this\n  provider. Authorization is layered on top of authentication in two independent\n  ways: a publication role model (OWNER / EDITOR / CONTRIBUTOR) and a\n  subscription gate (the target publication must be on the Pro plan).\n\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  token_location: header\n  header: Authorization\n  oauth2_flows: []\n  scopes: none\n  api_key_in: []\n  mtls: false\n\nschemes:\n  - name: PersonalAccessToken\n    type: http\n    scheme: bearer\n \
  \   in: header\n    header: Authorization\n    format: opaque\n    bearer_prefix_required: false\n    note: >-\n      The \"Bearer \" prefix is optional and case-insensitive. A deactivated user's\n      token is treated as unauthenticated.\n    issuance:\n      url: https://hashnode.com/settings/developer\n      path: Account Settings -> Developer / API tokens -> Generate new token\n      expiry: none documented\n      rotation: manual, from the dashboard\n    scope_of_power: >-\n      Full write access to every publication the user can act on - publish, edit,\n      and delete. Hashnode's own guidance is to treat it as a password.\n    handling_rules:\n      - Supply the token via the HASHNODE_PAT environment variable and interpolate it at request time.\n      - Never inline the literal token into a command string, file, script, or commit.\n      - Never ask a user to paste the token into a conversation and never print or log it.\n\naccess_matrix:\n  - operations: [post, feed, user, tag,\
  \ documentationProject, checkCustomDomainAvailability, checkSubdomainAvailability]\n    token_required: false\n    pro_required: false\n  - operations: [publication, searchPostsOfPublication, topCommenters]\n    token_required: false\n    pro_required: true\n    note: publication-scoped reads; FORBIDDEN when the target publication is not on Pro\n  - operations: [me]\n    token_required: true\n    pro_required: false\n  - operations: [draft, scheduledPost]\n    token_required: true\n    pro_required: true\n  - operations: [publishPost, updatePost, createDraft, updateDraft, publishDraft, submitDraftForReview, rejectDraftSubmission, deleteDraft]\n    token_required: true\n    pro_required: true\n  - operations: [createImageUploadURL]\n    token_required: true\n    pro_required: false\n\nroles:\n  model: UserPublicationRole\n  values:\n    - role: OWNER\n      capabilities: Creator of the publication; can do everything.\n    - role: EDITOR\n      capabilities: Customize the blog, approve/reject\
  \ posts, manage members.\n    - role: CONTRIBUTOR\n      capabilities: >-\n        Join and contribute an article. Cannot publish directly - must route writes\n        through createDraft -> submitDraftForReview, and cannot list other authors'\n        drafts.\n\nfailure_modes:\n  - condition: missing or invalid token on an authenticated operation\n    code: UNAUTHENTICATED\n  - condition: valid token, insufficient role\n    code: FORBIDDEN\n  - condition: valid token and role, publication not on Pro\n    code: FORBIDDEN\n    message: >-\n      Publication does not have an active Pro plan. Upgrade in your dashboard to\n      access this via the API.\n    retryable: false\n  - condition: draft the caller is not authorized for\n    code: NOT_FOUND\n    note: >-\n      Returned instead of FORBIDDEN by design, for privacy. Do not treat it as\n      \"retry with auth\".\n\nrelated:\n  errors: errors/hashnode-error-codes.yml\n  conventions: conventions/hashnode-conventions.yml\n  rate_limits:\
  \ rate-limits/hashnode-rate-limits.yml\n\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hashnode/refs/heads/main/authentication/hashnode-authentication.yml
summary_line: http · 1 scheme
tags:
- Blogging
- Developer Platform
- GraphQL
- Content Management
- Publications
- Newsletters
- Headless CMS
- Agent Skills
- Developer Community
- Documentation
---
