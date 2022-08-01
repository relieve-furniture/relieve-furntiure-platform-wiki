# Prismic.io

# Guide

### Content Modelling

- Create CustomType using SliceMachine
- Push CustomType to Prismic.io
- Create the page template
- Publish the content

### Using in Nextjs pages

- Generate Typescript type for you custom model

```bash
npm run primicTS:generate
```

- Fetch data using getByUID method of primic client in getServerSideProps

```typescript
const page = await client.getByUID('donate-form', 'register-donate', {
  lang: locale,
});
```

- return data:page.data as Page Props

```typescript
return {
  props: { data: page.data },
};
```

- Use the generate type
  If your custom type is namede form-document you can use as follow

```typescript
const Donate: FC<DonateFormDocument> = ({ data }: DonateFormDocument) => {
  return <p> {slices.data.slices[0]?.items[0].name} </p>;
};
```
