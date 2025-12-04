# Інтеграція GC з контейнерами та Kubernetes у .NET 10

.NET 10 GC оптимізований для роботи в контейнеризованих середовищах:

- Адаптація під обмеження пам’яті контейнера (cgroup limits);
- Автоматичне налаштування порогів алокації під memory QoS;
- Моніторинг GC через Kubernetes API для контролю інцидентів.

### Переваги:

- Стабільна робота .NET додатків у хмарі;
- Зменшення ризику OutOfMemoryError;
- Оптимізація ресурсів при масштабуванні.

### Джерела:

1. Kubernetes.io. "Best practices for .NET GC in containers", 2025.  
2. Azure Blog. "Running .NET workloads in containerized environments", 2025.
