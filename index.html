<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <title>Calculadora — Tarjeta de Crédito Garantizada con BTC</title>
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <script src="https://cdn.tailwindcss.com"></script>
  <style>
    .card {
      background: #ffffff;
      border-radius: 1rem;
      box-shadow: 0 10px 30px rgba(0,0,0,0.08);
    }
    .money {
      white-space: nowrap;
    }
  </style>
</head>
<body class="min-h-screen bg-slate-100 text-slate-900">
  <div class="max-w-5xl mx-auto px-4 py-8">
    <header class="mb-6 text-center">
      <h1 class="text-2xl sm:text-3xl font-bold text-slate-900">
        Calculadora — Tarjeta de Crédito Garantizada con BTC
      </h1>
      <p class="mt-2 text-sm sm:text-base text-slate-600">
        Simula el colateral en BTC y escenarios de LTV (70%, 80%, 90%) para una tarjeta de crédito garantizada.
      </p>
    </header>

    <!-- Configuración principal -->
    <section class="card p-4 sm:p-6 mb-6">
      <h2 class="text-lg sm:text-xl font-semibold mb-4 text-slate-900">
        Parámetros de la tarjeta
      </h2>

      <div class="grid gap-4 sm:grid-cols-2">
        <!-- Límite de la tarjeta -->
        <div class="space-y-2">
          <label for="limitInput" class="block text-sm font-medium text-slate-700">
            Límite de la tarjeta (USD) <span class="text-xs text-slate-500">(máx. $10,000)</span>
          </label>
          <div class="flex gap-2">
            <input
              id="limitInput"
              type="text"
              inputmode="decimal"
              autocomplete="off"
              class="flex-1 rounded-lg border border-slate-300 px-3 py-2 text-sm sm:text-base focus:outline-none focus:ring-2 focus:ring-blue-500 focus:border-blue-500"
              placeholder="10,000.00"
            />
            <button
              id="clearBtn"
              class="shrink-0 rounded-lg border border-slate-300 px-3 py-2 text-xs sm:text-sm font-medium text-slate-700 hover:bg-slate-50"
              type="button"
            >
              Limpiar
            </button>
          </div>
          <p id="limitError" class="text-xs text-red-500 h-4"></p>
        </div>

        <!-- Precio BTC -->
        <div class="space-y-2">
          <label for="priceInput" class="block text-sm font-medium text-slate-700">
            Precio del BTC (USD)
          </label>
          <div class="flex gap-2">
            <input
              id="priceInput"
              type="text"
              disabled
              class="flex-1 rounded-lg border border-slate-300 bg-slate-50 px-3 py-2 text-sm sm:text-base text-slate-700"
              placeholder="Actualiza para obtener el precio"
            />
            <button
              id="refreshBtn"
              class="shrink-0 rounded-lg bg-blue-600 px-3 py-2 text-xs sm:text-sm font-semibold text-white hover:bg-blue-700 disabled:opacity-60 disabled:cursor-not-allowed"
              type="button"
            >
              Actualizar precio
            </button>
          </div>
          <p id="apiError" class="text-xs text-red-500 h-4"></p>
        </div>
      </div>

      <div class="mt-4 flex items-center justify-between gap-4">
        <button
          id="calcBtn"
          class="rounded-lg bg-emerald-600 px-4 py-2 text-sm sm:text-base font-semibold text-white hover:bg-emerald-700 disabled:opacity-60 disabled:cursor-not-allowed"
          type="button"
          disabled
        >
          Calcular escenarios
        </button>
        <p class="text-xs sm:text-sm text-slate-500 text-right">
          El cálculo usa LTV inicial de <span class="font-semibold">70%</span> y escenarios de
          <span class="font-semibold">80%</span> (margin call) y <span class="font-semibold">90%</span> (bloqueo / liquidación).
        </p>
      </div>
    </section>

    <!-- Escenarios -->
    <section class="grid gap-4 sm:grid-cols-2 lg:grid-cols-4">
      <!-- Escenario 1 -->
      <article class="card p-4 flex flex-col">
        <h3 class="text-base sm:text-lg font-semibold text-slate-900 mb-1">
          Escenario 1 — LTV inicial 70%
        </h3>
        <p class="text-xs text-slate-500 mb-3">
          Colateral necesario en BTC para mantener un LTV del 70% sobre el límite de la tarjeta.
        </p>

        <div class="mt-auto space-y-2 text-sm sm:text-base">
          <div>
            <p class="text-xs text-slate-500">Unidades de BTC requeridas</p>
            <p id="btcUnits" class="font-mono text-sm sm:text-base text-slate-900">
              —
            </p>
          </div>
          <div>
            <p class="text-xs text-slate-500">Valor del colateral (USD)</p>
            <p id="btcValueUsd" class="money font-mono text-sm sm:text-base text-slate-900">
              —
            </p>
          </div>
        </div>
      </article>

      <!-- Escenario 2 -->
      <article class="card p-4 flex flex-col">
        <h3 class="text-base sm:text-lg font-semibold text-slate-900 mb-1">
          Escenario 2 — LTV · Margin Call (80%)
        </h3>
        <p class="text-xs text-slate-500 mb-3">
          Precio de BTC y valor del colateral cuando el LTV llega al 80% (señal de alerta).
        </p>

        <div class="mt-auto space-y-2 text-sm sm:text-base">
          <div>
            <p class="text-xs text-slate-500">Precio BTC con LTV al 80%</p>
            <p id="priceMC" class="money font-mono text-sm sm:text-base text-slate-900">
              —
            </p>
          </div>
          <div>
            <p class="text-xs text-slate-500">Valor del colateral (USD) al 80%</p>
            <p id="collMC" class="money font-mono text-sm sm:text-base text-slate-900">
              —
            </p>
          </div>
        </div>
      </article>

      <!-- Escenario 3 -->
      <article class="card p-4 flex flex-col">
        <h3 class="text-base sm:text-lg font-semibold text-slate-900 mb-1">
          Escenario 3 — LTV · Bloqueo (90%)
        </h3>
        <p class="text-xs text-slate-500 mb-3">
          Precio de BTC y colateral cuando el LTV alcanza el 90% y se bloquea la tarjeta.
        </p>

        <div class="mt-auto space-y-2 text-sm sm:text-base">
          <div>
            <p class="text-xs text-slate-500">Precio BTC con LTV al 90%</p>
            <p id="priceBlock" class="money font-mono text-sm sm:text-base text-slate-900">
              —
            </p>
          </div>
          <div>
            <p class="text-xs text-slate-500">Valor del colateral (USD) al 90%</p>
            <p id="collBlock" class="money font-mono text-sm sm:text-base text-slate-900">
              —
            </p>
          </div>
        </div>
      </article>

      <!-- Escenario 4 -->
      <article class="card p-4 flex flex-col">
        <h3 class="text-base sm:text-lg font-semibold text-slate-900 mb-1">
          Escenario 4 — Escenario de Liquidación (90%)
        </h3>
        <p class="text-xs text-slate-500 mb-2">
          Si al momento del bloqueo el saldo es igual o mayor a este valor, se ejecuta la liquidación.
        </p>

        <div class="mt-auto space-y-2 text-sm sm:text-base">
          <div>
            <p class="text-xs text-slate-500">Precio BTC considerado para la liquidación</p>
            <p id="priceLiq" class="money font-mono text-sm sm:text-base text-slate-900">
              —
            </p>
          </div>
          <div>
            <p class="text-xs text-slate-500">Valor del colateral (USD) al precio de bloqueo</p>
            <p id="collAtBlock" class="money font-mono text-sm sm:text-base text-slate-900">
              —
            </p>
          </div>
          <div>
            <p class="text-xs text-slate-500">
              Si al momento del bloqueo el saldo es igual o mayor a este valor, se ejecuta la liquidación.
            </p>
            <p id="dueAt90" class="money font-mono text-sm sm:text-base text-slate-900">
              —
            </p>
          </div>
        </div>
      </article>
    </section>
  </div>

  <script>
    (function () {
      const limitInput = document.getElementById('limitInput');
      const clearBtn = document.getElementById('clearBtn');
      const priceInput = document.getElementById('priceInput');
      const refreshBtn = document.getElementById('refreshBtn');
      const calcBtn = document.getElementById('calcBtn');

      const limitError = document.getElementById('limitError');
      const apiError = document.getElementById('apiError');

      const btcUnitsEl = document.getElementById('btcUnits');
      const btcValueUsdEl = document.getElementById('btcValueUsd');
      const priceMCEl = document.getElementById('priceMC');
      const collMCEl = document.getElementById('collMC');
      const priceBlockEl = document.getElementById('priceBlock');
      const collBlockEl = document.getElementById('collBlock');
      const priceLiqEl = document.getElementById('priceLiq');
      const collAtBlockEl = document.getElementById('collAtBlock');
      const dueAt90El = document.getElementById('dueAt90');

      let currentPrice = null;

      const usdFormatter = new Intl.NumberFormat('en-US', {
        style: 'currency',
        currency: 'USD',
        maximumFractionDigits: 2
      });

      const btcFormatter = new Intl.NumberFormat('en-US', {
        style: 'decimal',
        minimumFractionDigits: 8,
        maximumFractionDigits: 8
      });

      function parseLimitValue(value) {
        if (!value) return NaN;
        const cleaned = value.replace(/[^0-9.]/g, '');
        return parseFloat(cleaned);
      }

      function formatLimitInput() {
        const raw = parseLimitValue(limitInput.value);
        if (isNaN(raw)) {
          limitInput.value = '';
          return;
        }
        limitInput.value = raw.toLocaleString('en-US', {
          minimumFractionDigits: 2,
          maximumFractionDigits: 2
        });
      }

      function validateLimit() {
        const value = parseLimitValue(limitInput.value);
        if (!limitInput.value) {
          limitError.textContent = '';
          return null;
        }
        if (isNaN(value) || value <= 0) {
          limitError.textContent = 'Introduce un monto válido mayor que 0.';
          return null;
        }
        if (value > 10000) {
          limitError.textContent = 'El límite máximo permitido es $10,000.';
          return null;
        }
        limitError.textContent = '';
        return value;
      }

      function hasValidLimit() {
        const value = validateLimit();
        return typeof value === 'number' && !isNaN(value);
      }

      function hasValidPrice() {
        return typeof currentPrice === 'number' && !isNaN(currentPrice) && currentPrice > 0;
      }

      function updateCalcButtonState() {
        calcBtn.disabled = !(hasValidLimit() && hasValidPrice());
      }

      function clearResults() {
        btcUnitsEl.textContent = '—';
        btcValueUsdEl.textContent = '—';
        priceMCEl.textContent = '—';
        collMCEl.textContent = '—';
        priceBlockEl.textContent = '—';
        collBlockEl.textContent = '—';
        priceLiqEl.textContent = '—';
        collAtBlockEl.textContent = '—';
        dueAt90El.textContent = '—';
      }

      async function fetchPrice() {
        apiError.textContent = '';
        refreshBtn.disabled = true;
        refreshBtn.textContent = 'Actualizando...';
        try {
          const res = await fetch('https://api.coingecko.com/api/v3/simple/price?ids=bitcoin&vs_currencies=usd');
          if (!res.ok) {
            throw new Error('Respuesta no válida de la API');
          }
          const data = await res.json();
          const price = data?.bitcoin?.usd;
          if (typeof price !== 'number') {
            throw new Error('No se pudo obtener el precio.');
          }
          currentPrice = price;
          priceInput.value = usdFormatter.format(price);
        } catch (err) {
          console.error(err);
          apiError.textContent = 'No se pudo actualizar el precio. Intenta nuevamente.';
        } finally {
          refreshBtn.disabled = false;
          refreshBtn.textContent = 'Actualizar precio';
          updateCalcButtonState();
        }
      }

      function calculateScenarios() {
        const L = parseLimitValue(limitInput.value);
        const P = currentPrice;

        if (!L || !P) return;

        const u = L / (0.70 * P);
        const collateralUSD = L / 0.70;

        const priceMC = L / (0.80 * u);
        const collMC = u * priceMC;

        const priceBlock = L / (0.90 * u);
        const collBlock = u * priceBlock;

        const priceLiq = priceBlock;
        const collAtBlock = u * priceBlock;
        const dueAt90 = Math.min(L, 0.90 * collAtBlock);

        btcUnitsEl.textContent = btcFormatter.format(u);
        btcValueUsdEl.textContent = usdFormatter.format(collateralUSD);
        priceMCEl.textContent = usdFormatter.format(priceMC);
        collMCEl.textContent = usdFormatter.format(collMC);
        priceBlockEl.textContent = usdFormatter.format(priceBlock);
        collBlockEl.textContent = usdFormatter.format(collBlock);
        priceLiqEl.textContent = usdFormatter.format(priceLiq);
        collAtBlockEl.textContent = usdFormatter.format(collAtBlock);
        dueAt90El.textContent = usdFormatter.format(dueAt90);
      }

      // Event listeners
      limitInput.addEventListener('blur', () => {
        formatLimitInput();
        validateLimit();
        updateCalcButtonState();
      });

      limitInput.addEventListener('input', () => {
        validateLimit();
        updateCalcButtonState();
      });

      clearBtn.addEventListener('click', () => {
        limitInput.value = '';
        limitError.textContent = '';
        clearResults();
        updateCalcButtonState();
      });

      refreshBtn.addEventListener('click', () => {
        fetchPrice();
      });

      calcBtn.addEventListener('click', () => {
        calculateScenarios();
      });

      // Inicial
      clearResults();
    })();
  </script>
</body>
</html>
