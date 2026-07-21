# Product Passport Elements

Product Passport Elements is a standards-native circular-product registry demonstrating reusable Web Components for sustainability evidence, passport assembly, validation and publication.

[Watch the verified product demo](docs/demo.webm)

## Business problem and users

Manufacturers and market operators need interoperable durability, repair and material evidence across commerce, procurement and compliance applications. Product teams, conformity reviewers and circular-economy operators use reusable components instead of framework-specific silos.

## Key workflows

- Search and filter circular products.
- Inspect verification and circularity scores.
- Select products for passport assembly.
- Review attribute coverage and add validation context.
- Track passports through review, validation and publication.

## Lit and Web Components highlights

Lit reactive state/properties, Shadow DOM encapsulation, keyed rendering, a reusable reactive controller, composed custom events, typed element APIs and jsdom component tests. Components can interoperate with React, Vue, Angular or plain HTML hosts.

## Architecture and state flow

The workspace coordinates navigation and selection. `PassportController` owns publication lifecycle state. Leaf product/status elements accept typed properties and emit narrow framework-neutral events.

## Accessibility and responsive behaviour

Native inputs and buttons preserve keyboard behaviour across shadow roots, status is text-readable and component grids adapt to narrow host containers.

## Run and verify

```bash
npm ci
npm test
npm run build
npm run dev
```

## Structure

- `src/my-element.ts` — passport workspace
- `src/passport-controller.ts` — publication lifecycle
- `src/product-card.ts` — interoperable product element
- `src/status-card.ts` — reusable metric element
- `src/status-card.test.ts` — Shadow DOM/event tests

## Tradeoffs and roadmap

Evidence is illustrative. Production evolution includes ESPR schemas, identifiers, resolver APIs, signed evidence, access policies, lifecycle events, conformity workflows and framework-host examples.
