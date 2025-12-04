# Телеметрія та діагностика GC у .NET 10

.NET 10 GC підтримує **розширену телеметрію**:

- Метрики в реальному часі через EventCounters і ETW;
- Відстеження часу пауз, кількості зборів і використання пам’яті;
- Інтеграція з Application Insights та Prometheus для моніторингу.

### Переваги:

- Легко діагностувати проблеми з пам’яттю;
- Аналізувати навантаження у production;
- Оптимізувати конфігурації GC під конкретні додатки.

### Приклад коду для ETW:

```csharp
using System.Diagnostics.Tracing;

EventCounter gcPauseCounter = new EventCounter("gc-pause-time", MyEventSource.Log);
gcPauseCounter.WriteMetric(pauseTimeMs);
