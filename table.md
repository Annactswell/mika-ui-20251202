


profiles
  id: UUID
  userId: UUID
  nickname: TEXT
  avatarUrl: TEXT
  isPublic: BOOLEAN
  source: TEXT
  inviteCode: TEXT
  inviterCode: TEXT
  createdAt: TIMESTAMPZ
  updatedAt: TIMESTAMPZ
  deletedAt: TIMESTAMPZ
  metadata: JSONB

generations
  id: UUID
  userId: UUID
  type: TEXT
  prompt: TEXT
  url: TEXT
  createdAt: TIMESTAMPZ
  updatedAt: TIMESTAMPZ
  deletedAt: TIMESTAMPZ
  metadata: JSONB

subscriptions
  id: UUID
  userId: UUID
  planId: TEXT
  planCycle: TEXT
  status: TEXT
  startAt: TIMESTAMPZ
  endAt: TIMESTAMPZ
  usage: JSONB
  paymentId: UUID
  createdAt: TIMESTAMPZ
  updatedAt: TIMESTAMPZ
  deletedAt: TIMESTAMPZ
  metadata: JSONB

payments
  id: UUID
  userId: UUID
  amount: INT8
  currency: TEXT
  status: TEXT
  type: TEXT
  gateway: TEXT
  gatewayPaymentId: TEXT
  createdAt: TIMESTAMPZ
  updatedAt: TIMESTAMPZ
  deletedAt: TIMESTAMPZ
  metadata: JSONB

collections: 
  id: UUID
  userId: UUID
  targetType: TEXT
  targetId: UUID
  createdAt: TIMESTAMPZ
  metadata: JSONB









