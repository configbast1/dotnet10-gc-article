# Використання апаратного прискорення для GC у .NET 10

.NET 10 GC використовує сучасні апаратні можливості CPU для підвищення продуктивності:

- **Intel TSX** – зменшує блокування при паралельних операціях;
- **ARM SVE (Scalable Vector Extensions)** – прискорює маркування об’єктів;
- Спеціальні інструкції для швидкого оновлення card tables.

### Переваги:

- Підвищення продуктивності на багатоядерних CPU;
- Зменшення часу пауз при високих навантаженнях;
- Оптимізація для IoT та edge-додатків.

### Джерела:

1. Microsoft Docs. "Hardware acceleration for .NET GC", 2025.  
2. IEEE Transactions on Software Engineering, 2025. "Parallel and hardware-assisted GC algorithms".
