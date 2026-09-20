# EC-CUBE 41 Top Client Tasks & Enterprise Customization Master Guide (မြန်မာဘာသာ)

ဂျပန် EC-CUBE Real-world & Enterprise Project များတွင် Client (ဆိုင်ရှင် / ကုမ္ပဏီများ) ထံမှ လက်တွေ့ အများဆုံး တောင်းဆိုလေ့ရှိသော Task ၄၁ ခု (Forty-One Practical & Enterprise Client Requirements) ကို အဆင့်ဆင့် အကောင်အထည်ဖော်နည်း (Step-by-Step Implementation) နှင့် အဘယ်ကြောင့် ဤ Architecture/Function ကို အသုံးပြုရသနည်း (Why Use This) ဆိုသည့် အကြောင်းပြချက်များ အပြည့်အစုံ ပါဝင်သော လမ်းညွှန်ဖြစ်ပါသည်။

---

## 📋 Task စာရင်းချုပ် (Master Task List: Tasks 1 - 41)

### 🛍️ အပိုင်း ၁: ကုန်ပစ္စည်းနှင့် UI စိတ်ကြိုက်ပြင်ဆင်ခြင်း (Catalog & Frontend Tasks)

| # | Japanese Client Requirement | What you need to implement | Main EC-CUBE Skills | အသေးစိတ် လမ်းညွှန်ဖိုင် |
|---|-----------------------------|----------------------------|---------------------|-------------------|
| 1 | 商品一覧に商品コードを表示してください | Display product code | Twig, Entity | [01_display_product_code.md](./01_display_product_code.md) |
| 2 | 商品一覧にお気に入り数を表示してください | Favorite count | Repository, QueryBuilder, Twig | [02_favorite_count.md](./02_favorite_count.md) |
| 3 | お気に入り登録されている商品に印を表示してください | Favorite mark | Entity, Repository, Twig/Ajax | [03_favorite_mark.md](./03_favorite_mark.md) |
| 4 | 商品一覧に価格帯を表示してください | Price range | QueryBuilder, Twig | [04_price_range.md](./04_price_range.md) |
| 5 | 商品検索に価格範囲を追加してください | Min/max price search | FormType, Repository | [05_min_max_price_search.md](./05_min_max_price_search.md) |
| 6 | 商品一覧に並び替え機能を追加してください | Price/new/popularity sorting | QueryBuilder | [06_product_sorting.md](./06_product_sorting.md) |
| 7 | 商品一覧に在庫数を表示してください | Stock display | Entity, Twig | [07_stock_display.md](./07_stock_display.md) |
| 10 | 商品詳細に関連商品を表示してください | Related products | Repository, Twig | [10_related_products.md](./10_related_products.md) |
| 11 | 商品カテゴリを複数選択できるようにしてください | Multiple categories | Entity relationship, Form | [11_multiple_categories.md](./11_multiple_categories.md) |
| 22 | 特定の商品を会員限定にしてください | Member-only product | Security, Controller, Twig | [22_member_only_product.md](./22_member_only_product.md) |
| 26 | Ajaxでお気に入り登録できるようにしてください | No page reload favorite | Ajax, Controller, JSON | [26_ajax_favorite_toggle.md](./26_ajax_favorite_toggle.md) |

---

### ⚙️ အပိုင်း ၂: စီမံခန့်ခွဲမှုနှင့် ကုန်ပစ္စည်း/အော်ဒါ ထိန်းချုပ်ခြင်း (Admin & Operations)

| # | Japanese Client Requirement | What you need to implement | Main EC-CUBE Skills | အသေးစိတ် လမ်းညွှန်ဖိုင် |
|---|-----------------------------|----------------------------|---------------------|-------------------|
| 8 | 商品をCSVで一括登録できるようにしてください | Bulk product import | CSV, Entity, Validation | [08_bulk_product_csv_import.md](./08_bulk_product_csv_import.md) |
| 9 | 商品CSVに独自項目を追加してください | Custom CSV field | CSV, Entity | [09_custom_csv_field.md](./09_custom_csv_field.md) |
| 12 | 管理画面に新しいメニューを追加してください | New admin page/menu | Route, Controller, Twig, Permission | [12_admin_new_menu.md](./12_admin_new_menu.md) |
| 13 | 管理画面に検索条件を追加してください | Admin search | FormType, QueryBuilder | [13_admin_search_condition.md](./13_admin_search_condition.md) |
| 14 | 管理画面の商品一覧に項目を追加してください | New admin column | Controller, Twig | [14_admin_product_list_column.md](./14_admin_product_list_column.md) |
| 15 | お気に入り管理画面を作成してください | Favorite admin screen | Controller, Repository, Twig | [15_favorite_admin_screen.md](./15_favorite_admin_screen.md) |
| 16 | 注文一覧に独自の検索条件を追加してください | Custom order search | Form, Repository | [16_custom_order_search.md](./16_custom_order_search.md) |
| 17 | 注文ステータスを一括変更できるようにしてください | Bulk status update | Service, Transaction | [17_bulk_order_status_update.md](./17_bulk_order_status_update.md) |
| 20 | 顧客情報に独自項目を追加してください | Custom customer field | Entity, Migration, Form | [20_custom_customer_field.md](./20_custom_customer_field.md) |

---

### 💳 အပိုင်း ၃: အော်ဒါ၊ ငွေပေးချေမှုနှင့် ဝယ်ယူမှုအစီအစဉ်များ (Order, Checkout & Loyalty)

| # | Japanese Client Requirement | What you need to implement | Main EC-CUBE Skills | အသေးစိတ် လမ်းညွှန်ဖိုင် |
|---|-----------------------------|----------------------------|---------------------|-------------------|
| 18 | 注文完了時にメールを送信してください | Automatic email | Event Subscriber, Mailer | [18_order_complete_automatic_email.md](./18_order_complete_automatic_email.md) |
| 21 | 会員ランクによって価格を変更してください | Member pricing | Service, Entity, Event | [21_member_rank_pricing.md](./21_member_rank_pricing.md) |
| 23 | クーポン使用条件を追加してください | Custom coupon rules | Service, Validation | [23_custom_coupon_rules.md](./23_custom_coupon_rules.md) |
| 24 | 商品購入後にポイントを付与してください | Point system | Event Subscriber, Service | [24_purchase_point_system.md](./24_purchase_point_system.md) |
| 25 | 商品購入時に在庫を自動更新してください | Stock processing | Service, Transaction | [25_purchase_stock_auto_update.md](./25_purchase_stock_auto_update.md) |

---

### 🌐 အပိုင်း ၄: စနစ်စွမ်းဆောင်ရည်၊ API နှင့် ပြင်ပစနစ် ချိတ်ဆက်မှု (Performance & Batch)

| # | Japanese Client Requirement | What you need to implement | Main EC-CUBE Skills | အသေးစိတ် လမ်းညွှန်ဖိုင် |
|---|-----------------------------|----------------------------|---------------------|-------------------|
| 19 | 発送時に外部APIへ注文情報を送信してください | Shipping API | Event, Service, API | [19_shipping_external_api.md](./19_shipping_external_api.md) |
| 27 | 外部在庫システムと連携してください | Inventory API | API, Service, Command | [27_external_inventory_api_sync.md](./27_external_inventory_api_sync.md) |
| 28 | 毎日売上データを自動出力してください | Daily batch | Command, CSV | [28_daily_sales_batch_export.md](./28_daily_sales_batch_export.md) |
| 29 | 商品一覧の表示速度を改善してください | Performance optimization | QueryBuilder, N+1, Index, Cache | [29_product_list_performance_optimization.md](./29_product_list_performance_optimization.md) |
| 30 | 既存機能で500エラーが発生するので修正してください | Bug investigation/fix | Logs, Debug, all layers | [30_fix_500_error_investigation.md](./30_fix_500_error_investigation.md) |

---

### 🚀 အပိုင်း ၅: လုပ်ငန်းသုံး အဆင့်မြင့် ပေါင်းစပ်စနစ်များ (Enterprise Advanced Integrations: Tasks 31 - 41)

| # | Japanese Client Requirement | What you need to implement | Main EC-CUBE Skills | အသေးစိတ် လမ်းညွှန်ဖိုင် |
|---|-----------------------------|----------------------------|---------------------|-------------------|
| 31 | 注文から請求書を発行できるようにしてください | Invoice Management (インボイス制度対応PDF) | PDF, Entity, Tax Calculation | [31_invoice_management_pdf.md](./31_invoice_management_pdf.md) |
| 32 | 倉庫ごとに在庫を管理してください | Multiple Warehouses (複数拠点在庫・自動引当) | Multi-warehouse Entity, Routing Service | [32_multiple_warehouses_stock.md](./32_multiple_warehouses_stock.md) |
| 33 | 外部在庫システムとEC-CUBEの在庫を連携してください | Inventory Sync (API, Webhook, Retry) | Webhook, Retry Strategy, Fault-tolerance | [33_external_inventory_sync_webhook.md](./33_external_inventory_sync_webhook.md) |
| 34 | 基幹システムとEC-CUBEを連携してください | ERP/CRM Integration (顧客対応履歴・メモ管理) | CRM Memo Entity, Admin UI, CS History | [34_erp_crm_integration.md](./34_erp_crm_integration.md) |
| 35 | 商品ごとに配送可能日を設定してください | Delivery Date & Lead Time (リードタイム・カレンダー) | Delivery Calendar, Holiday, Cutoff | [35_delivery_date_leadtime_management.md](./35_delivery_date_leadtime_management.md) |
| 36 | 購入履歴からおすすめ商品を表示してください | Recommendation Engine (購入履歴レコメンド) | Collaborative Filtering, Association | [36_purchase_history_recommendation.md](./36_purchase_history_recommendation.md) |
| 37 | 売上・お気に入り・閲覧数をもとにランキングを作ってください | Product Ranking System (売上・PV・多軸ランキング) | Ranking Entity, Console Batch, Tabs UI | [37_multi_criteria_product_ranking.md](./37_multi_criteria_product_ranking.md) |
| 38 | 購入者だけがレビューできるようにしてください | Review & Rating (購入者限定レビュー・事前承認制) | Review Entity, Buyer Verification, Rating | [38_verified_buyer_review_system.md](./38_verified_buyer_review_system.md) |
| 39 | 会員登録・注文・キャンペーンをLINEと連携してください | LINE Integration (LINEログイン・Messaging API) | OAuth2 Social Login, Messaging Push | [39_line_social_integration.md](./39_line_social_integration.md) |
| 40 | 毎朝、対象注文を自動的に処理してください | Automated Daily Order Processing (朝次自動処理バッチ) | Symfony Console, Cron, Transaction | [40_automated_order_processing_batch.md](./40_automated_order_processing_batch.md) |
| 41 | 商品・顧客・注文データを外部システムとCSVで連携してください | Enterprise CSV Platform (大量データ連携基盤) | StreamedResponse, Generator, Upsert | [41_enterprise_csv_data_platform.md](./41_enterprise_csv_data_platform.md) |

---

## 🎯 သင်ခန်းစာ တစ်ခုချင်းစီတွင် ပါဝင်သော ဖွဲ့စည်းပုံ (Structure)

Task တစ်ခုချင်းစီကို ဖတ်ရှုလေ့လာရာတွင် အောက်ပါ စနစ်တကျ အချက် ၄ ချက်ဖြင့် တညီတညွတ်တည်း ရှင်းလင်းတင်ပြထားပါသည်:

1. **Client Requirement Analysis**: ဂျပန် Client တောင်းဆိုသော မူရင်းစာသားနှင့် အဓိပ္ပာယ် ရှင်းလင်းချက်။
2. **Architecture & "Why Use This"**: အဘယ်ကြောင့် ဤ Approach/Class/Function ကို ရွေးချယ်ရသနည်း (ဥပမာ - တိုက်ရိုက် Query မသုံးဘဲ Repository သုံးခြင်း၊ Controller မပြင်ဘဲ EventSubscriber သုံးခြင်း၊ Memory မပြည့်စေရန် Generator သုံးခြင်း စသည်)။
3. **Step-by-Step Implementation**: ဖိုင်တည်နေရာ၊ ရေးသားရမည့် PHP/Twig ကုဒ်နှင့် ရှင်းလင်းချက်များ။
4. **Key Pitfalls & Production Tips**: Real-world Project များတွင် အဖြစ်များသော ပြဿနာများ (N+1 Query, Deadlocks, Timeouts, Shift-JIS Encoding, Cache, Security) ကို ကြိုတင်ကာကွယ်နည်းများ။
