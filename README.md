Mini-RAG with Hallucination Detector 

Lightweight RAG pipeline with built-in hallucination detection.
No external API — runs in Google Colab with pure Python.

Pipeline: Question → Keyword Retrieval → Simulated Answer → Claim Check → Faithfulness Score → Citation

Features:
- 3-document knowledge base (Safety Policy, Remote Work, Data Protection)
- Keyword-based retrieval (no embeddings needed)
- 4 test questions: 2 grounded + 2 hallucinated
- Hallucination detector: checks every claim against source
- Citation generator with source attribution
- Metrics: Faithfulness, Hallucination Rate, Citation Accuracy

Results:
- Faithfulness: 0.33 | Hallucination Rate: 50% | Citation Accuracy: 50%
- Both hallucinations detected ✅
- Known limitation: keyword-matching misses semantic relevance → vector retrieval needed for production

Tech: Python 3, Google Colab, no external dependencies (re only)

Мини-RAG с детектором галлюцинаций

Лёгкий RAG-пайплайн со встроенным детектором галлюцинаций.
Без внешних API — работает в Google Colab на чистом Python.

Пайплайн: Вопрос → Поиск по ключевым словам → Симуляция ответа → Проверка утверждений → Оценка верности → Цитирование

Возможности:
- База знаний: 3 документа (Safety Policy, Remote Work, Data Protection)
- Поиск по ключевым словам (без векторных эмбеддингов)
- 4 тестовых вопроса: 2 опираются на документы, 2 галлюцинируют
- Детектор галлюцинаций: проверяет каждое утверждение на соответствие источнику
- Генератор цитирований с указанием источника
- Метрики: Faithfulness, Hallucination Rate, Citation Accuracy

Результаты:
- Faithfulness: 0.33 | Hallucination Rate: 50% | Citation Accuracy: 50%
- Обе галлюцинации обнаружены ✅
- Ограничение: keyword-matching не учитывает семантику → для продакшена нужен векторный поиск

Технологии: Python 3, Google Colab, без внешних зависимостей (только re)
