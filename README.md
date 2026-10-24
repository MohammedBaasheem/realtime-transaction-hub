# خريطة الطريق الشاملة لتكامل الأنظمة المحاسبية (.NET Integration Mastery)

مرحباً بك! تم تصميم هذا المستودع خصيصاً ليأخذك خطوة بخطوة من مرحلة المبتدئ إلى مستوى الاحتراف كـ **Integration Specialist** في بيئات الأنظمة المالية والمحاسبية (ERP Systems) باستخدام **.NET 8**.

تم تنظيم العمل في **مشروعين مستقلين تماماً**، وكل مشروع يمتلك حزمة وثائق كاملة متطابقة الترقيم (من 01 إلى 06) تغطي كافة التفاصيل:

---

## 🚀 المشروع الأول: محرك الربط اللحظي الموثوق (Real-Time Transaction Hub)
يختص بمعالجة العمليات الفردية فور حدوثها (من نقاط البيع POS أو المتاجر) وترحيلها لحظياً للـ ERP مع ضمان منع التكرار وعدم ضياع أي قرش.

* 📄 [01- وثيقة المعمارية وتدفق البيانات](file:///e:/.net%20web%20api/integration%20in%20.net/Project1_RealTime_TransactionHub/docs/01-architecture-and-flow.md): المخطط الهيكلي، مسار الطلب، معمارية Clean Architecture، ومخطط التسلسل (Sequence Diagram).
* 📄 [02- دليل المفاهيم المحاسبية للمطور](file:///e:/.net%20web%20api/integration%20in%20.net/Project1_RealTime_TransactionHub/docs/02-accounting-domain-guide.md): القيد المزدوج، شجرة الحسابات، قيود الضريبة 15% وعمولات البطاقات، وقاموس مصطلحات الـ GL, Sub-ledger, Cost Centers.
* 📄 [03- دليل أنماط الموثوقية والتكامل](file:///e:/.net%20web%20api/integration%20in%20.net/Project1_RealTime_TransactionHub/docs/03-resilience-and-patterns.md): شرح تطبيقي لـ (Idempotency, Transactional Outbox, Polly v8 Retry & Circuit Breaker, Dead-Letter Queue).
* 📄 [04- مواصفات الـ API ونماذج البيانات](file:///e:/.net%20web%20api/integration%20in%20.net/Project1_RealTime_TransactionHub/docs/04-api-contracts-and-schemas.md): نماذج الـ JSON للفواتير والقيود المحاسبية، الـ Headers، وأكواد الأخطاء.
* 📄 [05- دليل التشغيل والاختبار العملي](file:///e:/.net%20web%20api/integration%20in%20.net/Project1_RealTime_TransactionHub/docs/05-runbook-and-testing.md): خطوات التشغيل وسيناريوهات اختبار سقوط الـ ERP وتكرار الطلبات بـ curl و Postman.
* 📄 [06- دليل المقابلة الشخصية والدفاع عن المشروع](file:///e:/.net%20web%20api/integration%20in%20.net/Project1_RealTime_TransactionHub/docs/06-interview-defense-guide.md): كيف تقدم المشروع في دقيقتين وأهم 7 أسئلة متوقعة مع إجاباتها النموذجية.

---

## 🔄 المشروع الثاني: محرك المزامنة بالدفعات والتسوية المالية (Batch Sync & Reconciliation)
يختص بمعالجة الكميات الضخمة من البيانات في الخلفية، التعامل مع قواعد البيانات القديمة والملفات، وإجراء المطابقة الآلية بين سجلات المبيعات وحسابات البنك.

* 📄 [01- وثيقة المعمارية وتصميم المعالجة بالدفعات](file:///e:/.net%20web%20api/integration%20in%20.net/Project2_Batch_Reconciliation/docs/01-architecture-and-batch-design.md): معمارية المهام المجدولة، معمارية Pipeline & Adapters، ومخطط سير المطابقة.
* 📄 [02- دليل التسوية والمطابقة المالية](file:///e:/.net%20web%20api/integration%20in%20.net/Project2_Batch_Reconciliation/docs/02-financial-reconciliation-guide.md): خوارزمية المطابقة التلقائية، اكتشاف الفروقات والغياب البنكي، وقاموس مصطلحات التسوية البنكية.
* 📄 [03- دليل التعامل مع قواعد البيانات القديمة والملفات](file:///e:/.net%20web%20api/integration%20in%20.net/Project2_Batch_Reconciliation/docs/03-legacy-db-and-file-processing.md): القراءة بـ Dapper من جداول الـ Legacy، وتحليل ملفات الـ CSV البنكية و XML الفواتير.
* 📄 [04- دليل الجدولة والعمليات بالجملة](file:///e:/.net%20web%20api/integration%20in%20.net/Project2_Batch_Reconciliation/docs/04-hangfire-and-bulk-operations.md): إعداد Hangfire، مهام الـ Cron، وسرعة الـ `SqlBulkCopy` الفائقة مقارنة بـ EF Core.
* 📄 [05- دليل التشغيل والاختبار العملي](file:///e:/.net%20web%20api/integration%20in%20.net/Project2_Batch_Reconciliation/docs/05-runbook-and-testing.md): تشغيل لوحة التحكم Hangfire Dashboard واختبار رفع كشف الحساب واكتشاف الفروقات.
* 📄 [06- دليل المقابلة الشخصية والدفاع عن المشروع](file:///e:/.net%20web%20api/integration%20in%20.net/Project2_Batch_Reconciliation/docs/06-interview-defense-guide.md): أهم أسئلة المقابلات حول الأنظمة القديمة والـ Bulk Processing والمطابقة.
