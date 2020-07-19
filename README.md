:construction: in Development :construction:

# class-validator

```typescript
  switch (paramMetadata.paramType) {
    case "body":
      try {
        args[paramMetadata.index] = await transformAndValidate(
          paramMetadata.type,
          req.body,
          {
            transformer: paramMetadata.classTransform
              ? paramMetadata.classTransform
              : void 0,
            validator: paramMetadata.validatorOptions,
          }
        );
      } catch (error) {
        throw new ValidationError(error);
      }
```
