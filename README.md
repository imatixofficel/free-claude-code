# به نام پروردگار

<div align="center">

<h1>
  <picture>
    <source media="(prefers-color-scheme: light)" srcset="assets/free-claude-code-wordmark-light.svg">
    <img src="assets/free-claude-code-wordmark-dark.svg" alt="Free Claude Code" width="610">
  </picture>
</h1>

[![مجوز: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-2e7d32.svg?style=for-the-badge)](https://github.com/Alishahryar1/free-claude-code/blob/main/LICENSE)
[![پایتون 3.14](https://img.shields.io/badge/python-3.14-3776ab.svg?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/downloads/)
[![مدیر بسته: uv](assets/package-manager-uv.svg)](https://github.com/astral-sh/uv)
[![تست: Pytest](https://img.shields.io/badge/Testing-Pytest-ad1457.svg?style=for-the-badge)](https://github.com/Alishahryar1/free-claude-code/actions/workflows/tests.yml)
[![بررسی نوع: Ty](https://img.shields.io/badge/Type%20Checker-ty-fdd835.svg?style=for-the-badge)](https://pypi.org/project/ty/)
[![فرمت‌کننده: Ruff](https://img.shields.io/badge/Formatter-ruff-bf4b00.svg?style=for-the-badge)](https://github.com/astral-sh/ruff)
[![لاگ: Loguru](https://img.shields.io/badge/logging-loguru-00695c.svg?style=for-the-badge)](https://github.com/Delgan/loguru)

[⚡ شروع سریع](#quick-start) · [🔌 ارائه‌دهندگان](#choose-a-provider) · [🖥️ کلاینت‌ها](#connect-your-client) · [🧩 یکپارچه‌سازی‌ها](#optional-integrations) · [⚙️ مدیریت](#manage-your-installation)

</div>

<p align="center">
  <em>پروژه مستقل متن‌باز. وابسته به Anthropic نیست و توسط آن تأیید نشده است. Claude و Claude Code علائم تجاری Anthropic هستند.</em>
</p>

---

## 🎯 چه چیزی دریافت می‌کنید

- 💰 **۶۱ ارائه‌دهنده سازگار با شرایط استفاده. بیش از ۱.۳ میلیارد توکن رایگان در هر ماه.** از مدل‌های رایگان، پولی، اشتراکی و محلی از یک رابط جستجوپذیر واحد استفاده کنید بدون اینکه حساب خود را در خطر بیندازید. FCC از شرایط ارائه‌دهندگان پیروی می‌کند و اگر یکپارچه‌سازی‌ها دیگر مجاز نباشند، آن‌ها را حذف می‌کند.
- 🤖 **۱۲ عامل کدنویسی. یک کاتالوگ مدل.** [Claude Code](https://code.claude.com/docs/en/overview)، [Codex](https://github.com/openai/codex)، [Pi](https://github.com/earendil-works/pi)، [OpenCode](https://github.com/anomalyco/opencode)، [Cline](https://github.com/cline/cline)، [Hermes](https://github.com/NousResearch/hermes-agent)، [DeepSeek Harness](https://github.com/deepseek-ai/deepseek-harness)، [Grok Build](https://github.com/xai-org/grok-build)، [Muse Code](https://research.meta.ai/blog/introducing-muse-code-and-muse-spark-1-2/)، [Aider](https://aider.chat/)، [Antigravity CLI](https://antigravity.google/docs/getting-started/)، یا [VS Code Chat](https://code.visualstudio.com/) را با مدل‌های FCC خود اجرا کنید.
- 🛡️ **در طول قطعی‌های ارائه‌دهنده به کدنویسی ادامه دهید.** پس از اتمام تلاش‌های مجدد، FCC به‌طور خودکار مدل پیکربندی‌شده بعدی شما را امتحان می‌کند بدون اینکه مجبور باشید نوبت را دوباره شروع کنید. این در همه کلاینت‌ها کار می‌کند.
- 📉 **تا ۹۰٪ کاهش مصرف توکن.** فیلترهای اختیاری [RTK](https://github.com/rtk-ai/rtk) خروجی معمول دستورات را فیلتر می‌کنند، و [Headroom](https://github.com/headroomlabs-ai/headroom) نتایج ابزار را فشرده می‌کند.
- 🌐 **جلسات بومی کد در مرورگر شما.** یک پوشه انتخاب کنید و Codex را در مرورگر با پشتیبانی بلادرنگ و پس‌زمینه اجرا کنید. آزادانه ارائه‌دهنده/مدل را در همان جلسه تغییر دهید. پشتیبانی از تغییر هارنس در همان جلسه به‌زودی!
- 📱 **ترمینال، دسکتاپ، IDE یا گوشی.** از طریق لانچرهای بومی، [VS Code](https://code.visualstudio.com/)، [Codex App](https://learn.chatgpt.com/docs/app)، [JetBrains](https://www.jetbrains.com/)، [Discord](https://discord.com/) یا [Telegram](https://telegram.org/) کار کنید.
- 🎤 **یادداشت صوتی وارد کنید. کد دریافت کنید.** با عامل خود با استفاده از [Whisper](https://github.com/openai/whisper) محلی یا [NVIDIA NIM](https://docs.nvidia.com/nim/speech/latest/asr/deploy-asr-models/whisper.html) صحبت کنید.
- 🧠 **قابلیت‌های عامل دست‌نخورده می‌مانند.** پاسخ‌های استریم، استفاده از ابزارها، حفظ تفکر درهم‌تنیده بومی برای حداکثر عملکرد، ارسال تصاویر، و مسیریابی [Fable](https://www.anthropic.com/claude/fable)، [Opus](https://www.anthropic.com/claude/opus)، [Sonnet](https://www.anthropic.com/claude/sonnet)، و [Haiku](https://www.anthropic.com/claude/haiku) به‌صورت مستقل با مدل‌های سازگار.

> ⚠️ در دسترس بودن و محدودیت‌های سطح رایگان توسط هر ارائه‌دهنده کنترل می‌شود و ممکن است تغییر کند.

<div align="center">
  <img src="assets/pic.png" alt="Claude Code running with Free Claude Code" width="700">
  <p><em>Claude Code در حال اجرا با FCC.</em></p>
</div>

<div align="center">
  <img src="assets/browser-code-session.png" alt="Native Codex browser session in FCC, showing model controls and a repository exploration" width="700">
  <p><em>یک جلسه بومی Codex در رابط مرورگر FCC.</em></p>
</div>

---

## ⚡ شروع سریع

<a id="install"></a>

### ۱️⃣ نصب

**macOS / Linux:**

```bash
curl -fsSL "https://raw.githubusercontent.com/Alishahryar1/free-claude-code/main/scripts/install.sh" | sh
```

**Windows PowerShell:**

```powershell
& ([scriptblock]::Create((irm "https://raw.githubusercontent.com/Alishahryar1/free-claude-code/main/scripts/install.ps1")))
```

> 💡 وقتی از شما پرسیده شد، حداقل یک عامل کدنویسی انتخاب کنید و به‌صورت اختیاری بهینه‌سازی توکن [RTK](https://github.com/rtk-ai/rtk) + [Headroom](https://github.com/headroomlabs-ai/headroom) را برای عامل‌های پشتیبانی‌شده فعال کنید.

### ۲️⃣ شروع FCC

| سیستم‌عامل | روش |
| --- | --- |
| 🪟 **Windows** | **Free Claude Code** را از دسکتاپ یا منوی Start باز کنید. |
| 🍎 **macOS** | **Free Claude Code** را از دسکتاپ یا پوشه Applications باز کنید. |
| 🐧 **Linux** | دستور `fcc-server` را اجرا کنید. |

> ℹ️ FCC پس از شروع، رابط مدیریت (Admin UI) را باز می‌کند. در Windows و macOS، از آیکون tray یا نوار منو برای باز کردن Admin، راه‌اندازی مجدد یا خروج استفاده کنید. هنگام استفاده از `fcc-server`، ترمینال آن را باز نگه دارید.

<a id="nvidia-nim-provider"></a>

### ۳️⃣ پیکربندی NVIDIA NIM

1. 🔑 یک کلید API در [build.nvidia.com/settings/api-keys](https://build.nvidia.com/settings/api-keys) ایجاد کنید.
2. 🌐 URL رابط مدیریت را از لاگ سرور باز کنید.
3. 🖱️ NVIDIA NIM را در **Providers** باز کنید، روی **Add key** کلیک کنید، کلید را جای‌گذاری کنید و روی **Save** کلیک کنید.
4. 🎛️ `MODEL` را روی پیش‌فرض `nvidia_nim/nvidia/nemotron-3-ultra-550b-a55b` بگذارید، یا مدل دیگری را از منوی کشویی جستجو و انتخاب کنید.
5. ✅ روی **Apply** کلیک کنید تا انتخاب مدل ذخیره شود.

> 🔒 برای محافظت از پروکسی محلی با توکن bearer، **Proxy Authentication** را در Admin فعال کنید.

<div align="center">
  <img src="assets/admin-page.png" alt="Free Claude Code Admin UI" width="700">
</div>

### ۴️⃣ عامل کدنویسی خود را اجرا کنید

| عامل | دستور |
| --- | --- |
| 🟣 **Claude Code** | `fcc-claude` |
| ⚫ **Codex** | `fcc-codex` |
| 🔵 **Pi** | `fcc-pi` |
| 🟢 **OpenCode 2** | `fcc-opencode` |
| 🟠 **Cline** | `fcc-cline` |
| 🟡 **Hermes** | `fcc-hermes` |
| 🟤 **DeepSeek Harness Web** | `fcc-dsh` |
| 🔴 **Grok Build** | `fcc-grok` |
| 🟪 **Muse Code** | `fcc-muse` |
| 🟩 **Aider** | `fcc-aider` |
| ⬜ **Antigravity CLI** *(ابتدا در صفحه Integrations متصل شوید)* | `fcc-agy` |

<a id="model-picker"></a>

<div align="center">
  <img src="assets/cc-model-picker.png" alt="Claude Code model picker showing FCC models" width="700">
  <p><em>یک مدل FCC را از انتخابگر بومی <code>/model</code> Claude Code انتخاب کنید.</em></p>
</div>

---

## 🔌 انتخاب یک ارائه‌دهنده

1. 📎 یک لینک ارائه‌دهنده در جدول زیر باز کنید برای کلید، مدل‌ها یا دستورالعمل‌های راه‌اندازی آن.
2. ⚙️ در رابط مدیریت، تنظیمات ذکرشده را پیکربندی کنید. برای دسترسی اشتراک OpenAI / ChatGPT، به‌جای آن از **Providers → OAuth providers** استفاده کنید.
3. 🔍 منوی کشویی `MODEL` را جستجو کنید و یک مدل انتخاب کنید. اگر ارائه‌دهنده نمی‌تواند مدل‌ها را فهرست کند، `<provider-id>/<exact-provider-model-id>` را به‌صورت دستی وارد کنید.
4. ✅ روی **Apply** کلیک کنید.

> 💡 **اختیاری:** یک لیست مرتب **Fallback Models** در **Model Config** اضافه کنید. این برای هر کلاینت متصل اعمال می‌شود. یک درخواست ناموفق ممکن است قبل از موفقیت به بیش از یک ارائه‌دهنده برسد و از مصرف آن‌ها استفاده کند.

> 🔑 مودال‌های ارائه‌دهنده از کلیدهای API شماره‌گذاری‌شده پشتیبانی می‌کنند. از **Add key** استفاده کنید، ردیف‌ها را حذف کنید، یا دستگیره‌های آن‌ها را برای تغییر ترتیب بکشید. FCC از کلید ۱ استفاده می‌کند.

> 🛠️ برای یک نقطه پایانی API دیگر، **Providers → Custom providers → Add provider** را باز کنید. URL پایه API، کلیدهای اختیاری و فرمت API آن را وارد کنید. **Model IDs** را خالی بگذارید تا مدل‌ها به‌طور خودکار کشف شوند، یا یک شناسه مدل upstream در هر خط وارد کنید. ذخیره کنید، سپس یک مدل را در **Model Config** انتخاب کنید.

<details>
<summary><strong>📚 کاتالوگ ارائه‌دهندگان</strong> (کلیک کنید)</summary>

| ارائه‌دهنده | تنظیم رابط مدیریت | مثال `MODEL` |
| --- | --- | --- |
| [NVIDIA NIM](https://build.nvidia.com/settings/api-keys) | `NVIDIA_NIM_API_KEY` | `nvidia_nim/nvidia/nemotron-3-ultra-550b-a55b` |
| [OpenRouter](https://openrouter.ai/keys) | `OPENROUTER_API_KEY` | `open_router/openrouter/free` |
| [Groq](https://console.groq.com/keys) | `GROQ_API_KEY` | `groq/llama-3.3-70b-versatile` |
| [ClinePass](https://docs.cline.bot/getting-started/clinepass) | `CLINE_API_KEY` | `cline_pass/cline-pass/kimi-k3` |
| [OpenAI / ChatGPT](https://learn.chatgpt.com/docs/auth) | اتصال ChatGPT در رابط مدیریت | `openai/<model-id>` |
| [OpenAI API](https://platform.openai.com/api-keys) | `OPENAI_API_KEY` | `openai_api/gpt-5.6-sol` |
| [GitHub Copilot](https://docs.github.com/en/copilot/how-tos/copilot-sdk/auth/authenticate) | اتصال GitHub Copilot در رابط مدیریت | `github_copilot/<model-id>` |
| [xAI (Grok)](https://console.x.ai/team/default/api-keys) | `XAI_API_KEY` | `xai/grok-4.5` |
| [Alibaba Cloud](https://www.alibabacloud.com/help/en/model-studio/get-api-key) | `ALIBABA_CLOUD_API_KEY` | `alibaba_cloud/<model-id>` |
| [QwenCloud Token Plan](https://home.qwencloud.com/api-keys) | `QWENCLOUD_API_KEY` | `qwencloud/qwen3.7-plus` |
| [QwenCloud Coding Plan](https://home.qwencloud.com/api-keys) | `QWENCLOUD_CODING_API_KEY` | `qwencloud_coding/qwen3.7-plus` |
| [Together AI](https://api.together.ai/settings/api-keys) | `TOGETHER_API_KEY` | `together/zai-org/GLM-5.2` |
| [DeepInfra](https://deepinfra.com/dash/api_keys) | `DEEPINFRA_API_KEY` | `deepinfra/deepseek-ai/DeepSeek-V4-Flash` |
| [SiliconFlow](https://cloud.siliconflow.com/account/ak) | `SILICONFLOW_API_KEY` | `siliconflow/Qwen/Qwen3-32B` |
| [Nebius Token Factory](https://tokenfactory.nebius.com/project/api-keys) | `NEBIUS_API_KEY` | `nebius/Qwen/Qwen3-30B-A3B` |
| [Chutes](https://chutes.ai/docs/getting-started/authentication) | `CHUTES_API_KEY` | `chutes/Qwen/Qwen3-32B-TEE` |
| [Featherless AI](https://featherless.ai/account/api-keys) | `FEATHERLESS_API_KEY` | `featherless/Qwen/Qwen3-32B` |
| [Agnes AI](https://agnes-ai.com/) | `AGNES_API_KEY` | `agnes/agnes-2.0-flash` |
| [ZenMux](https://zenmux.ai/platform/pay-as-you-go) | `ZENMUX_API_KEY` | `zenmux/deepseek/deepseek-v4-flash-free` |
| [W&B Inference](https://wandb.ai/settings) | `WANDB_API_KEY` | `wandb/openai/gpt-oss-20b` |
| [Anthropic](https://platform.claude.com/settings/keys) | `ANTHROPIC_API_KEY` | `anthropic/<model-id>` |
| [Azure OpenAI](https://learn.microsoft.com/azure/foundry/openai/how-to/chatgpt) | `AZURE_OPENAI_API_KEY` و `AZURE_OPENAI_BASE_URL` | `azure_openai/<deployment-name>` |
| [Google AI Studio (Gemini)](https://aistudio.google.com/apikey) | `GEMINI_API_KEY` | `gemini/models/gemini-3.1-flash-lite` |
| [Google Vertex AI](https://cloud.google.com/vertex-ai/generative-ai/docs/start/openai) | `VERTEX_PROJECT_ID` + ADC | `vertex/google/gemini-3.5-flash` |
| [DeepSeek](https://platform.deepseek.com/api_keys) | `DEEPSEEK_API_KEY` | `deepseek/deepseek-chat` |
| [Mistral La Plateforme](https://console.mistral.ai/) | `MISTRAL_API_KEY` | `mistral/devstral-small-latest` |
| [Mistral Codestral](https://console.mistral.ai/) | `CODESTRAL_API_KEY` | `mistral_codestral/codestral-latest` |
| [OpenCode Zen](https://opencode.ai/auth) | `OPENCODE_API_KEY` | `opencode_zen/gpt-5.3-codex` |
| [OpenCode Go](https://opencode.ai/auth) | `OPENCODE_API_KEY` | `opencode_go/minimax-m2.7` |
| [Vercel AI Gateway](https://vercel.com/docs/ai-gateway/models-and-providers) | `AI_GATEWAY_API_KEY` | `vercel/openai/gpt-5.5` |
| [Amazon Bedrock](https://console.aws.amazon.com/bedrock/) | `AWS_BEARER_TOKEN_BEDROCK` | `bedrock/openai.gpt-oss-120b` |
| [Hugging Face Inference Providers](https://huggingface.co/settings/tokens) | `HUGGINGFACE_API_KEY` | `huggingface/Qwen/Qwen3-Coder-480B-A35B-Instruct:fastest` |
| [Cohere](https://dashboard.cohere.com/api-keys) | `COHERE_API_KEY` | `cohere/command-a-plus-05-2026` |
| [Wafer](https://wafer.ai/) | `WAFER_API_KEY` | `wafer/DeepSeek-V4-Pro` |
| [Kimi API](https://platform.moonshot.ai/console/api-keys) | `KIMI_API_KEY` | `kimi/kimi-k2.5` |
| [Kimi Code](https://www.kimi.com/code/console) | `KIMI_CODE_API_KEY` | `kimi_code/k3` |
| [MiniMax](https://platform.minimax.io/user-center/basic-information/interface-key) | `MINIMAX_API_KEY` | `minimax/MiniMax-M3` |
| [Cerebras Inference](https://cloud.cerebras.ai/) | `CEREBRAS_API_KEY` | `cerebras/gpt-oss-120b` |
| [SambaNova](https://cloud.sambanova.ai/apis) | `SAMBANOVA_API_KEY` | `sambanova/Meta-Llama-3.3-70B-Instruct` |
| [Kilo.ai](https://kilo.ai) | `KILO_API_KEY` | `kilo/kilo-auto/free` |
| [Fireworks AI](https://fireworks.ai/account/api-keys) | `FIREWORKS_API_KEY` | `fireworks/accounts/fireworks/models/llama-v3p3-70b-instruct` |
| [Novita AI](https://novita.ai/settings/key-management) | `NOVITA_API_KEY` | `novita/deepseek/deepseek-v4-flash-0731` |
| [Cloudflare Workers AI](https://developers.cloudflare.com/workers-ai/) | `CLOUDFLARE_API_TOKEN` و `CLOUDFLARE_ACCOUNT_ID` | `cloudflare/@cf/moonshotai/kimi-k2.6` |
| [Z.ai Coding Plan](https://z.ai/manage-apikey/apikey-list) | `ZAI_API_KEY` | `zai/glm-5.2` |
| [Z.ai API (pay as you go)](https://z.ai/manage-apikey/apikey-list) | `ZAI_API_KEY` | `zai_api/glm-4.7-flash` |
| [TokenRouter](https://www.tokenrouter.com/) | `TOKENROUTER_API_KEY` | `tokenrouter/moonshotai/kimi-k3-free` |
| [NaraRoute](https://router.bynara.id/) | `NARAROUTE_API_KEY` | `nararoute/kimi-k3-free` |
| [Poolside AI](https://platform.poolside.ai/) | `POOLSIDE_API_KEY` | `poolside/poolside/laguna-s-2.1` |
| [LLM7.io](https://dash.llm7.io/) | `LLM7_API_KEY` | `llm7/default` |
| [Scaleway](https://console.scaleway.com/iam/api-keys) | `SCW_SECRET_KEY` | `scaleway/deepseek/deepseek-v4-flash` |
| [Lightning AI](https://lightning.ai/) | `LIGHTNING_API_KEY` | `lightning/lightning-ai/Qwen3.8-27B` |
| [Experiential Labs](https://platform.experientiallabs.ai/) | `EXPLABS_API_KEY` | `experiential/union-alpha` |
| [Cheaper Inference](https://cheaperinference.com/signup) | `CHEAPER_INFERENCE_API_KEY` | `cheaperinference/gpt-5.4-mini` |
| [OrcaRouter](https://www.orcarouter.ai/) | `ORCAROUTER_API_KEY` | `orcarouter/deepseek/deepseek-v4-flash-free` |
| [Atlas Cloud](https://console.atlascloud.ai/api-keys) | `ATLASCLOUD_API_KEY` | `atlascloud/deepseek-ai/deepseek-v4-flash` |
| [xKiro](https://xkiro.com/) | `XKIRO_API_KEY` | `xkiro/qwen/qwen3.7-flash:free` |
| [Opper](https://platform.opper.ai/) | `OPPER_API_KEY` | `opper/claude-sonnet-4-6` |
| [Ollama Cloud](https://ollama.com/settings/keys) | `OLLAMA_API_KEY` | `ollama_cloud/qwen3-coder:480b` |
| [LM Studio](https://lmstudio.ai/) | `LM_STUDIO_BASE_URL` | `lmstudio/<model-id>` |
| [llama.cpp](https://github.com/ggml-org/llama.cpp) | `LLAMACPP_BASE_URL` | `llamacpp/<model-id>` |
| [Ollama](https://ollama.com/) | `OLLAMA_BASE_URL` | `ollama/<model-tag>` |

</details>

<details>
<summary><strong>🔧 راه‌اندازی مخصوص ارائه‌دهنده</strong> (کلیک کنید)</summary>

- 🔐 **OpenAI / ChatGPT** از اشتراک ChatGPT شما به‌جای کلید API استفاده می‌کند. از **Providers → OAuth providers → OpenAI / ChatGPT → Connect** در رابط مدیریت متصل شوید و ورود را از طریق مرورگر کامل کنید. پس از اتصال، عامل در حال اجرا را مجدداً راه‌اندازی کنید.
- 🔐 **Anthropic** از یک کلید API جداگانه صورتحساب‌شده استفاده می‌کند. آن را در **Providers → Cloud providers → Anthropic → Configure** اضافه کنید، سپس یک مدل کشف‌شده انتخاب کنید. کلیدهای چندفضای‌کاری همچنین به `ANTHROPIC_WORKSPACE_ID` نیاز دارند.
- 🔐 **OpenAI API** از یک کلید API پلتفرم جداگانه استفاده می‌کند. آن را در **Providers → Cloud providers → OpenAI API → Configure** وارد کنید. لیست مدل ممکن است شامل شناسه‌هایی باشد که نمی‌توانند درخواست‌های کدنویسی را مدیریت کنند. یک مدل تولید متن انتخاب کنید.
- 🐙 **GitHub Copilot** از حساب و اشتراک GitHub وارد‌شده شما استفاده می‌کند. [Copilot CLI 1.0.83](https://github.com/github/copilot-cli/releases/tag/v1.0.83) را روی PATH نصب کنید، سپس **Providers → OAuth providers → GitHub Copilot → Connect** را انتخاب کنید. ورود را کامل کنید، سپس یک `github_copilot/<model-id>` از انتخابگر مدل انتخاب کنید. مدل‌ها و سهمیه‌های موجود به اشتراک و سیاست‌های سازمان شما بستگی دارد. پس از اتصال، عامل در حال اجرا را مجدداً راه‌اندازی کنید.
- ☁️ **Azure OpenAI** از نام‌های استقرار (deployment) از منبع شما استفاده می‌کند. `AZURE_OPENAI_BASE_URL` را روی نقطه پایانی کامل v1 آن تنظیم کنید، مانند `https://YOUR-RESOURCE-NAME.openai.azure.com/openai/v1/`، و یک استقرار انتخاب کنید که از Chat Completions پشتیبانی می‌کند. اگر نام استقرار در منوی کشویی مدل ظاهر نشد، آن را به‌عنوان یک اسلاگ مدل سفارشی وارد کنید.
- 🌬️ **Mistral Codestral** از یک کلید جداگانه از Mistral La Plateforme استفاده می‌کند.
- 🌙 **Kimi Code** از `kimi_code/` استفاده می‌کند. کلیدهای اعتباری **Kimi API** از `kimi/` استفاده می‌کنند. طرح‌های Kimi Code برای استفاده شخصی تعاملی از عامل کدنویسی تحت [دستورالعمل‌های اجتماعی Kimi](https://www.kimi.com/code/docs/en/kimi-code/community-guidelines.html) هستند.
- 🏯 **Alibaba Cloud** از یک کلید pay-as-you-go Model Studio استفاده می‌کند و پیش‌فرض آن سنگاپور است. برای منطقه یا فضای‌کاری دیگر، `ALIBABA_CLOUD_BASE_URL` را روی [نقطه پایانی سازگار با OpenAI](https://www.alibabacloud.com/help/en/model-studio/base-url) آن تنظیم کنید که به `/compatible-mode/v1` ختم می‌شود. کلید و نقطه پایانی باید از یک منطقه استفاده کنند.
- 🐉 **QwenCloud Coding Plan** از `qwencloud_coding/` استفاده می‌کند. **QwenCloud Token Plan** از `qwencloud/` استفاده می‌کند. کلیدها و نقاط پایانی قابل تعویض نیستند. Coding Plan برای استفاده محلی، شخصی و تعاملی از عامل کدنویسی تحت [شرایط Coding Plan](https://www.alibabacloud.com/help/en/model-studio/coding-plan) است.
- 🔀 **OpenCode Zen** و **OpenCode Go** در `OPENCODE_API_KEY` مشترک هستند اما از پیشوندهای صریح مدل `opencode_zen/` و `opencode_go/` استفاده می‌کنند.
- 🪨 **Amazon Bedrock**: `BEDROCK_BASE_URL` را روی URL همان منطقه‌ای که کلید API در آن قرار دارد تنظیم کنید و یکی از مدل‌های فهرست‌شده را انتخاب کنید.
- 🧭 **Vertex AI** از Google Application Default Credentials به‌جای کلید API استفاده می‌کند. به‌صورت محلی، یک بار `gcloud auth application-default login` را اجرا کنید. فایل‌های حساب سرویس و حساب‌های سرویس متصل نیز کار می‌کنند. `VERTEX_PROJECT_ID` را تنظیم کنید، و به‌صورت اختیاری `VERTEX_LOCATION` را از پیش‌فرض `global` آن تغییر دهید.
- ☁️ **Cloudflare** به هم توکن API و هم شناسه حساب نیاز دارد.
- 🦙 **Ollama Cloud**: از شناسه‌های مدل دقیقی که در انتخابگر مدل نشان داده شده‌اند استفاده کنید. Ollama محلی از پیشوند جداگانه `ollama/` استفاده می‌کند.
- ⚠️ مدل‌های دارای قابلیت ابزار را برای عامل‌های کدنویسی ترجیح دهید. مدل‌های محلی همچنین به زمینه کافی برای اعلان سیستم عامل و تعاریف ابزار نیاز دارند.

</details>

<details>
<summary><strong>🏠 راه‌اندازی ارائه‌دهنده محلی</strong> (کلیک کنید)</summary>

> 🔄 FCC به‌طور خودکار مدل‌ها را از سرورهای محلی در حال اجرا در زمان شروع کشف می‌کند. اگر سروری را بعداً شروع کردید، روی **Refresh models** در Admin کلیک کنید تا مدل‌های آن به انتخابگر اضافه شوند.

### 🎨 LM Studio

سرور محلی LM Studio را شروع کنید، یک مدل دارای قابلیت ابزار بارگذاری کنید، و از شناسه مدلی که LM Studio نشان می‌دهد با پیشوند `lmstudio/` استفاده کنید. URL پیش‌فرض `http://localhost:1234/v1` است.

### 🦙 llama.cpp

`llama-server` را با API سازگار با OpenAI Chat Completions و زمینه کافی برای مدل شروع کنید. از شناسه مدل محلی با پیشوند `llamacpp/` استفاده کنید. `LLAMACPP_BASE_URL` پیش‌فرض `http://localhost:8080/v1` است.

### 🐑 Ollama

```bash
ollama pull llama3.1
ollama serve
```

از تگ نشان داده شده توسط `ollama list` با پیشوند `ollama/` استفاده کنید. `OLLAMA_BASE_URL` پیش‌فرض `http://localhost:11434` است.

> 💡 کارت‌های ارائه‌دهنده نقطه پایانی بررسی‌شده و زمان پاسخ را نشان می‌دهند، با یک پیام مفید وقتی سرور محلی در دسترس نیست. پس از شروع سرور یا اصلاح تنظیمات آن، روی **Test** کلیک کنید تا مدل‌های آن بازخوانی شوند.

</details>

<details>
<summary><strong>🎚️ مسیریابی اختیاری سطح مدل</strong> (کلیک کنید)</summary>

> `MODEL` جایگزین (fallback) برای هر درخواست است. یک مدل برای `MODEL_FABLE`، `MODEL_OPUS`، `MODEL_SONNET`، یا `MODEL_HAIKU` انتخاب کنید تا یک سطح خاص Claude Code را بازنویسی کنید. **None** را انتخاب کنید تا از `MODEL` استفاده شود.

در **Admin UI → Model Config**، **Fallback Models** را به ترتیبی که FCC باید در صورت شکست مدل انتخاب‌شده امتحان کند اضافه کنید. هر fallback تلاش استدلال خود را دارد: **Inherit**، **Off**، **From client**، **Low**، **Medium**، **High**، **X-High**، یا **Max**.

یک مدل، تلاش و شماره کلید API را در ردیف پایین انتخاب کنید، سپس روی **+** کلیک کنید. **Key 1**، **Key 2**، و غیره به کلیدهای شماره‌گذاری‌شده فعلی در تنظیمات آن ارائه‌دهنده اشاره دارند. انتخاب‌ها را در جای خود ویرایش کنید، دستگیره را برای تغییر ترتیب بکشید، یا برای حذف یک fallback روی دکمه قرمز سطل زباله کلیک کنید.

> 🧬 **Inherit** تنظیم استدلال حل‌شده درخواست اصلی را حفظ می‌کند. **From client** از تلاش یا بودجه توکن ارسال‌شده توسط عامل کدنویسی شما استفاده می‌کند و تنظیمات جهانی یا سطح را دور می‌زند. می‌توانید همان مدل را با شماره کلید دیگری انتخاب کنید.

</details>

<details>
<summary><strong>🧠 کنترل استدلال</strong> (کلیک کنید)</summary>

**Admin UI → Model Config → Model Routing** را باز کنید و یک تلاش کنار هر مدل انتخاب کنید. **Default Effort** از **From client** شروع می‌شود. Fable، Opus، Sonnet، و Haiku از **Inherit** شروع می‌کنند.

| انتخاب | رفتار |
| --- | --- |
| 🎯 **From client** | از تلاش ارسال‌شده توسط عامل کدنویسی شما استفاده کنید. اگر هیچ‌کدام ارسال نشود، پیش‌فرض ارائه‌دهنده را حفظ کنید. |
| ⏸️ **Off** | درخواست غیرفعال کردن استدلال. |
| 📊 **Low**، **Medium**، **High**، **X-High**، یا **Max** | کلاینت را با سطح استدلال انتخاب‌شده بازنویسی کنید. |
| 🔄 **Inherit** | بازنویسی‌های سطح از Default Effort استفاده می‌کنند. Fallbackها تلاش حل‌شده درخواست اصلی را حفظ می‌کنند. |

</details>

<a id="connect-your-client"></a>

## 🖥️ اتصال کلاینت شما

> 🚀 لانچرهای FCC به‌طور خودکار سرور را شروع می‌کنند.

برای یکپارچه‌سازی‌های ویرایشگر و اپلیکیشن، کلاینت را نصب کنید، FCC را شروع کنید، سپس **Admin UI → Integrations** را باز کنید و روی **Connect** در کارت آن کلیک کنید.

- 🟦 **Claude Code در VS Code**: [افزونه Claude Code](https://marketplace.visualstudio.com/items?itemName=anthropic.claude-code) را نصب کنید.
- 💬 **VS Code Chat**: آخرین [VS Code](https://code.visualstudio.com/) را نصب کنید، متصل شوید، و یک مدل FCC را در انتخابگر مدل Chat داخلی آن انتخاب کنید.
- 🖥️ **Claude Desktop**: [Claude Desktop](https://claude.ai/download) را نصب کنید. قبل از اتصال یا قطع اتصال، آن را کاملاً ببندید، سپس دوباره باز کنید. قطع اتصال به ورود عادی Claude بازمی‌گردد.
- ⚫ **Codex در VS Code و App**: [افزونه Codex](https://marketplace.visualstudio.com/items?itemName=openai.chatgpt) یا Codex App را نصب کنید.
- 🐋 **DeepSeek Harness Desktop**: برنامه را یک بار قبل از اتصال نصب و باز کنید. یک جلسه جدید شروع کنید تا از مدل‌های FCC استفاده کنید.
- 🧩 **Claude Code در JetBrains ACP**: Claude Agent را در JetBrains AI Assistant نصب کنید و یک بار آن را شروع کنید، سپس روی **Connect** در FCC کلیک کنید. IDE را دوباره باز کنید، **Claude Code (FCC)** را انتخاب کنید و یک چت جدید شروع کنید. پس از به‌روزرسانی عامل توسط JetBrains، FCC را قبل از شروع چت جدید مجدداً راه‌اندازی کنید. نیاز به یک IDE محلی در مکان‌های نصب استاندارد آن دارد.

> 🔁 پس از اتصال، VS Code را بارگذاری مجدد کنید یا برنامه/IDE را مجدداً راه‌اندازی کنید. در Codex و Claude Desktop، یک مدل FCC را از انتخابگر مدل انتخاب کنید. وقتی FCC تنظیمات به‌روزشده را گزارش می‌دهد، کلاینت را بارگذاری مجدد یا راه‌اندازی مجدد کنید. برای حذف یکپارچه‌سازی از **Disconnect** در همان کارت استفاده کنید.

> ✅ برای تکمیل جداگانه آنبوردینگ Claude Code، **Admin UI → Integrations → Claude Code onboarding** را باز کنید و روی **Complete onboarding** کلیک کنید. اتصال Claude Code در VS Code نیز آنبوردینگ را کامل می‌کند.

> ⚠️ FCC را روی همان کامپیوتر و در همان محیط کاربری کلاینتی که پیکربندی می‌کنید اجرا کنید.

<a id="optional-integrations"></a>

## 🧩 یکپارچه‌سازی‌های اختیاری

> ⚙️ یکپارچه‌سازی‌ها را از **Admin UI → Messaging** پیکربندی کنید، سپس روی **Apply** کلیک کنید.

<details>
<summary><strong>🎮 ربات Discord</strong> (کلیک کنید)</summary>

1. 🤖 یک ربات در [Discord Developer Portal](https://discord.com/developers/applications) ایجاد کنید.
2. ✅ **Message Content Intent** را فعال کنید و آن را با مجوزهای خواندن، ارسال، تاریخچه پیام، و **Manage Messages** دعوت کنید تا `/clear` بتواند اعلان‌های کاربر را حذف کند.
3. ⚙️ **Messaging Platform** را روی **discord** تنظیم کنید.
4. 🔑 **Discord Bot Token**، **Allowed Discord Channels**، و یک **Allowed Directory** مطلق وارد کنید.
5. ✅ تنظیمات را اعمال کنید و در صورت درخواست، سرور را مجدداً راه‌اندازی کنید.

</details>

<details>
<summary><strong>📨 ربات Telegram</strong> (کلیک کنید)</summary>

1. 🤖 یک ربات با [@BotFather](https://t.me/BotFather) ایجاد کنید.
2. 🆔 شناسه عددی کاربری خود را از [@userinfobot](https://t.me/userinfobot) دریافت کنید. در گروه‌ها، به ربات مجوز حذف پیام بدهید.
3. ⚙️ **Messaging Platform** را روی **telegram** تنظیم کنید.
4. 🔑 **Telegram Bot Token**، **Allowed Telegram User ID**، و یک **Allowed Directory** مطلق وارد کنید.
5. ✅ تنظیمات را اعمال کنید و در صورت درخواست، سرور را مجدداً راه‌اندازی کنید.

</details>

### 💬 دستورات پیام‌رسانی

| استفاده | رفتار |
| --- | --- |
| 📊 `/stats` | وضعیت جلسه را نشان دهید. |
| ⏹️ `/stop` مستقل | همه کارها را لغو کنید. |
| ↩️ پاسخ با `/stop` | فقط درخواست انتخاب‌شده را لغو کنید در حالی که سایر درخواست‌های صف‌شده ادامه می‌یابند. |
| 🗑️ `/clear` مستقل | همه مکالمات FCC و پیام‌های آن‌ها را در این چت پاک کنید. |
| 🧹 پاسخ با `/clear` | پیام انتخاب‌شده و زنجیره پاسخ‌های به آن را حذف کنید. سایر مکالمات را نگه دارید. |

<details>
<summary><strong>🎤 یادداشت‌های صوتی</strong> (کلیک کنید)</summary>

> 🎙️ پشتیبانی رونویسی NVIDIA NIM در هر نصب گنجانده شده است. در **Admin UI → Messaging → Voice**، یادداشت‌های صوتی را فعال کنید، `nvidia_nim` را انتخاب کنید، و یک مدل پشتیبانی‌شده انتخاب کنید. کلید **NVIDIA NIM API** خود را در صفحه Providers پیکربندی کنید.

برای Whisper محلی روی CPU یا CUDA، نصب‌کننده را با گزینه صوت محلی دوباره اجرا کنید:

**macOS / Linux — Whisper محلی روی CPU یا CUDA:**

```bash
curl -fsSL "https://raw.githubusercontent.com/Alishahryar1/free-claude-code/main/scripts/install.sh" | sh -s -- --voice-local
```

**macOS / Linux — Whisper محلی با CUDA 13.0:**

```bash
curl -fsSL "https://raw.githubusercontent.com/Alishahryar1/free-claude-code/main/scripts/install.sh" | sh -s -- --voice-local --torch-backend cu130
```

**Windows PowerShell — Whisper محلی روی CPU یا CUDA:**

```powershell
& ([scriptblock]::Create((irm "https://raw.githubusercontent.com/Alishahryar1/free-claude-code/main/scripts/install.ps1"))) -VoiceLocal
```

**Windows PowerShell — Whisper محلی با CUDA 13.0:**

```powershell
& ([scriptblock]::Create((irm "https://raw.githubusercontent.com/Alishahryar1/free-claude-code/main/scripts/install.ps1"))) -VoiceLocal -TorchBackend cu130
```

> 🔁 پس از نصب پشتیبانی محلی، `fcc-server` را مجدداً راه‌اندازی کنید. در **Admin UI → Messaging → Voice**، یادداشت‌های صوتی را فعال کنید، `cpu` یا `cuda` را انتخاب کنید، و مدل Whisper را انتخاب کنید. مدل‌های محلی gated به `HUGGINGFACE_API_KEY` نیاز دارند.

</details>

---

## ⚙️ مدیریت نصب شما

> 🔍 برای بررسی نسخه نصب‌شده بدون شروع FCC، `fcc-server --version` را اجرا کنید.

### 🔄 به‌روزرسانی

همه دستورات FCC در حال اجرا را متوقف کنید، سپس اجرا کنید:

```sh
fcc-update
```

> ✅ به‌روزرسانی، نسخه پایدار بررسی‌شده FCC را با نصب‌کننده منطبق آن نصب می‌کند. برای نصب مجدد FCC یا تغییر اجزای اختیاری در حالی که از قبل به‌روز هستید، نصب‌کننده را مستقیماً اجرا کنید. برای پشتیبانی صوت محلی، `--voice-local` (macOS/Linux) یا `-VoiceLocal` (Windows) را اضافه کنید، به‌همراه گزینه `--torch-backend` یا `-TorchBackend` خود در صورت استفاده.

### 🎼 Muse Code روی Windows بومی

برای نصب یا به‌روزرسانی فقط Muse Code:

```powershell
& ([scriptblock]::Create((irm "https://raw.githubusercontent.com/Alishahryar1/free-claude-code/main/scripts/install-muse.ps1")))
```

برای حذف نسخه Muse Code نصب‌شده توسط FCC، با نگه داشتن داده‌های آن:

```powershell
& ([scriptblock]::Create((irm "https://raw.githubusercontent.com/Alishahryar1/free-claude-code/main/scripts/uninstall-muse.ps1")))
```

> ℹ️ حذف FCC، Muse Code را نصب‌شده باقی می‌گذارد.

### 🗑️ حذف نصب

> ⚠️ قبل از حذف نصب، هر دستور FCC در حال اجرا را متوقف کنید و برنامه‌های دسکتاپ/ویرایشگر متصل را ببندید.

**❌ حذف می‌کند:**
- Free Claude Code، شامل لانچر دسکتاپ و دستورات آن
- `~/.fcc/`

**✅ نگه می‌دارد:**
- uv و Python
- عامل‌های کدنویسی شما، RTK، و Headroom

**macOS / Linux:**

```bash
curl -fsSL "https://raw.githubusercontent.com/Alishahryar1/free-claude-code/main/scripts/uninstall.sh" | sh
```

**Windows PowerShell:**

```powershell
& ([scriptblock]::Create((irm "https://raw.githubusercontent.com/Alishahryar1/free-claude-code/main/scripts/uninstall.ps1")))
```

---

## 🔗 پیوندهای پروژه

> 🩺 برای یک مشکل پس از نصب، دستور زیر را اجرا کنید و خروجی آن را در گزارش باگ خود جای‌گذاری کنید.

```bash
fcc-doctor
```

- 🐛 [گزارش باگ یا درخواست ویژگی](https://github.com/Alishahryar1/free-claude-code/issues)
- 🤝 [راهنمای مشارکت](CONTRIBUTING.md)

---

## 📜 مجوز

> **GNU Affero General Public License version 3 only** (`AGPL-3.0-only`). برای جزئیات به [LICENSE](LICENSE) مراجعه کنید.

---

## 📋 چیت شیت دستورات پرکاربرد

| دستور | کار |
| --- | --- |
| `fcc-server` | 🚀 شروع سرور + باز کردن Admin UI |
| `fcc-server --version` | 🔍 نمایش نسخه نصب‌شده |
| `fcc-claude` | 🟣 اجرای Claude Code با مدل‌های FCC |
| `fcc-codex` | ⚫ اجرای Codex |
| `fcc-pi` | 🔵 اجرای Pi |
| `fcc-opencode` | 🟢 اجرای OpenCode 2 |
| `fcc-cline` | 🟠 اجرای Cline |
| `fcc-hermes` | 🟡 اجرای Hermes |
| `fcc-dsh` | 🟤 اجرای DeepSeek Harness Web |
| `fcc-grok` | 🔴 اجرای Grok Build |
| `fcc-muse` | 🟪 اجرای Muse Code |
| `fcc-aider` | 🟩 اجرای Aider |
| `fcc-agy` | ⬜ اجرای Antigravity CLI |
| `fcc-update` | 🔄 به‌روزرسانی FCC |
| `fcc-doctor` | 🩺 عیب‌یابی و گزارش وضعیت |

---


