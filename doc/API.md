# **Relieve Furniture Platform**

## API

### Rest Api


```
└── api/
    └── export/
    │   └── models
    │   └── orders
    ├── graphql
    ├── sendMail
    ├── auth/
    │   ├── buyback
    │   ├── login
    │   ├── logout
    │   ├── me
    │   └── signup
    ├── campaign/
    │   ├── update/
    │   │   └── [param]
    │   ├── create
    │   ├── delete
    │   ├── orders
    │   ├── pickupList
    │   └── report
    ├── product/
    │   ├── update/
    │   │   └── [param]
    │   ├── add
    │   ├── remove
    │   └── validate
    ├── stripe/
    │   ├── checkout_invoice
    │   └── webhook
    ├── user/
    │   ├── createBuyer
    │   ├── createDonator
    │   ├── delete
    │   ├── update
    │   └── validate
    ├── contact/
    │   ├── create
    │   ├── delete
    │   └── update
    ├── image/
    │   ├── delete
    │   └── upload
    └── orders/
       └── details

```

### GraphQL API

Endpoint:

<env.url>/api/graphql

For the reference go to [Apollo studio](https://studio.apollographql.com/sandbox/schema/reference)
