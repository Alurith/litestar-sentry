# litestar-sentry
A WIP Litestar-Sentry integration

## How to use
Import ```LitestarIntegration``` then add this:
```python
sentry_sdk.init(
    dsn=settings.SENTRY_DNS,
    integrations=[
        LitestarIntegration(),
    ],
    # Set traces_sample_rate to 1.0 to capture 100%
    # of transactions for performance monitoring.
    traces_sample_rate=1.0,
)
```
