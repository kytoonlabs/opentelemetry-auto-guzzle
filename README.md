# OpenTelemetry Guzzle auto-instrumentation

Please read https://opentelemetry.io/docs/instrumentation/php/automatic/ for instructions on how to
install and configure the extension and SDK.

## Overview

Auto-instrumentation hooks are registered via composer.

* create spans automatically for each Guzzle request that is sent (sync or async)
* add a `traceparent` header to the request to facilitate distributed tracing

## Configuration

The extension can be disabled via [runtime configuration](https://opentelemetry.io/docs/instrumentation/php/sdk/#configuration):

```shell
OTEL_PHP_DISABLED_INSTRUMENTATIONS=guzzle
```
