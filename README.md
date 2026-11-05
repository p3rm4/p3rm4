<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1000 420" width="100%" height="100%">
  <defs>
    <linearGradient id="termBg" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#090B10" />
      <stop offset="60%" stop-color="#0D1117" />
      <stop offset="100%" stop-color="#18070B" />
    </linearGradient>
    <linearGradient id="headerBg" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#161B22" />
      <stop offset="100%" stop-color="#24090E" />
    </linearGradient>
    <linearGradient id="crimsonBar" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#8B0000" />
      <stop offset="100%" stop-color="#E63946" />
    </linearGradient>
    <linearGradient id="cyanBar" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#0077B6" />
      <stop offset="100%" stop-color="#00F5D4" />
    </linearGradient>
    <filter id="glow" x="-20%" y="-20%" width="140%" height="140%">
      <feGaussianBlur stdDeviation="3.5" result="blur" />
      <feComposite in="SourceGraphic" in2="blur" operator="over" />
    </filter>
    <pattern id="hudGrid" width="24" height="24" patternUnits="userSpaceOnUse">
      <path d="M 24 0 L 0 0 0 24" fill="none" stroke="#E63946" stroke-width="0.4" stroke-opacity="0.14" />
    </pattern>

    <style>
      .mono { font-family: 'Fira Code', 'JetBrains Mono', Consolas, 'Courier New', monospace; }
      .line1 { opacity: 0; animation: appear 0.35s ease forwards 0.3s; }
      .line2 { opacity: 0; animation: appear 0.35s ease forwards 1.0s; }
      .line3 { opacity: 0; animation: appear 0.35s ease forwards 1.8s; }
      .line4 { opacity: 0; animation: appear 0.35s ease forwards 2.5s; }
      .line5 { opacity: 0; animation: appear 0.35s ease forwards 3.3s; }
      .line6 { opacity: 0; animation: appear 0.35s ease forwards 4.4s; }
      .line7 { opacity: 0; animation: appear 0.35s ease forwards 5.1s; }
      .cursor { animation: blink 0.9s step-end infinite; }
      .pulse { animation: pulseGlow 2.2s ease-in-out infinite; }
      @keyframes appear {
        from { opacity: 0; }
        to { opacity: 1; }
      }
      @keyframes blink {
        0%, 100% { opacity: 1; }
        50% { opacity: 0; }
      }
      @keyframes pulseGlow {
        0%, 100% { opacity: 0.9; }
        50% { opacity: 0.3; }
      }
    </style>
  </defs>

  <!-- Outer Frame -->
  <rect x="2" y="2" width="996" height="416" rx="14" fill="url(#termBg)" stroke="#8B0000" stroke-width="2" />
  <rect x="2" y="2" width="996" height="416" rx="14" fill="url(#hudGrid)" />

  <!-- Top Window Bar -->
  <path d="M 2 16 Q 2 2 16 2 L 984 2 Q 998 2 998 16 L 998 44 L 2 44 Z" fill="url(#headerBg)" />
  <line x1="2" y1="44" x2="998" y2="44" stroke="#8B0000" stroke-width="1.2" />

  <!-- Window Traffic Lights -->
  <circle cx="26" cy="23" r="6.5" fill="#FF5F56" />
  <circle cx="48" cy="23" r="6.5" fill="#FFBD2E" />
  <circle cx="70" cy="23" r="6.5" fill="#27C93F" />

  <!-- Window Title -->
  <text x="500" y="28" class="mono" font-size="13" font-weight="600" fill="#C9D1D9" text-anchor="middle" letter-spacing="1">
    root@p3rm4:~/ultra-instinct-core — zsh (120x42)
  </text>

  <!-- Live Telemetry Badge Top Right -->
  <rect x="850" y="11" width="132" height="24" rx="12" fill="#120608" stroke="#E63946" stroke-width="1" />
  <circle cx="868" cy="23" r="4.5" fill="#2EA043" class="pulse" />
  <text x="924" y="27" class="mono" font-size="10.5" font-weight="700" fill="#F1FAEE" text-anchor="middle" letter-spacing="1.2">LIVE KERNEL</text>

  <!-- Vertical Split Divider -->
  <line x1="635" y1="44" x2="635" y2="418" stroke="#8B0000" stroke-width="1" stroke-dasharray="5,5" />

  <!-- ================= LEFT PANEL: ANIMATED TERMINAL ================= -->
  <g transform="translate(26, 76)" class="mono" font-size="13">

    <!-- Step 1: Command 1 -->
    <g class="line1">
      <text x="0" y="0">
        <tspan fill="#E63946" font-weight="700">root@p3rm4</tspan><tspan fill="#8B949E">:</tspan><tspan fill="#58A6FF">~/systems</tspan><tspan fill="#F1FAEE"> $ ./init_warrior.sh --user="Hassan Sial"</tspan>
      </text>
    </g>

    <!-- Step 2: Output 1 -->
    <g class="line2">
      <text x="0" y="26">
        <tspan fill="#2EA043" font-weight="700">[✓] IDENTITY VERIFIED: </tspan><tspan fill="#F1FAEE" font-weight="600">Hassan Sial (@p3rm4)</tspan>
      </text>
      <text x="0" y="48">
        <tspan fill="#2EA043" font-weight="700">[✓] CLEARANCE LEVEL:   </tspan><tspan fill="#E63946" font-weight="700">MASTERED ULTRA INSTINCT // ARCHITECT</tspan>
      </text>
    </g>

    <!-- Step 3: Command 2 -->
    <g class="line3">
      <text x="0" y="82">
        <tspan fill="#E63946" font-weight="700">root@p3rm4</tspan><tspan fill="#8B949E">:</tspan><tspan fill="#58A6FF">~/systems</tspan><tspan fill="#F1FAEE"> $ cargo run --release --bin neural-cluster</tspan>
      </text>
    </g>

    <!-- Step 4: Output 2 -->
    <g class="line4">
      <text x="0" y="108">
        <tspan fill="#8B949E">  Compiling </tspan><tspan fill="#F1FAEE">p3rm4-ai-engine v4.9.0 (/core/llm-orchestrator)</tspan>
      </text>
      <text x="0" y="130">
        <tspan fill="#8B949E">  Compiling </tspan><tspan fill="#F1FAEE">zero-trust-sec v3.2.1 (/core/defense-matrix)</tspan>
      </text>
      <text x="0" y="152">
        <tspan fill="#8B949E">  Compiling </tspan><tspan fill="#F1FAEE">auto-bot-grid v2.8.4 (/core/playwright-cluster)</tspan>
      </text>
    </g>

    <!-- Step 5: Live Progress Bars (Explicit Y coordinates, no transform override) -->
    <g class="line5">
      <!-- Bar 1 -->
      <text x="0" y="188" fill="#58A6FF" font-weight="600">▸ AI Agent Mesh</text>
      <rect x="165" y="176" width="265" height="12" rx="4" fill="#161B22" stroke="#30363D" stroke-width="1" />
      <rect x="165" y="176" width="265" height="12" rx="4" fill="url(#crimsonBar)">
        <animate attributeName="width" values="0;265" dur="1.6s" begin="3.3s" fill="freeze" />
      </rect>
      <text x="444" y="188" fill="#2EA043" font-weight="700">100% ONLINE</text>

      <!-- Bar 2 -->
      <text x="0" y="216" fill="#58A6FF" font-weight="600">▸ Full-Stack Core</text>
      <rect x="165" y="204" width="265" height="12" rx="4" fill="#161B22" stroke="#30363D" stroke-width="1" />
      <rect x="165" y="204" width="258" height="12" rx="4" fill="url(#cyanBar)">
        <animate attributeName="width" values="0;258" dur="1.8s" begin="3.5s" fill="freeze" />
      </rect>
      <text x="444" y="216" fill="#00F5D4" font-weight="700">99.9% READY</text>

      <!-- Bar 3 -->
      <text x="0" y="244" fill="#58A6FF" font-weight="600">▸ Defense Shield</text>
      <rect x="165" y="232" width="265" height="12" rx="4" fill="#161B22" stroke="#30363D" stroke-width="1" />
      <rect x="165" y="232" width="265" height="12" rx="4" fill="url(#crimsonBar)">
        <animate attributeName="width" values="0;265" dur="1.5s" begin="3.7s" fill="freeze" />
      </rect>
      <text x="444" y="244" fill="#E63946" font-weight="700">ENFORCED</text>
    </g>

    <!-- Step 6: Telemetry Status Box -->
    <g class="line6">
      <rect x="0" y="264" width="580" height="34" rx="6" fill="#1A080C" stroke="#8B0000" stroke-width="1" />
      <text x="14" y="286" fill="#F1FAEE" font-size="12">
        <tspan fill="#E63946" font-weight="700">⚡ STATUS: </tspan>
        <tspan fill="#C9D1D9">All distributed nodes active | Latency: </tspan>
        <tspan fill="#2EA043" font-weight="700">0.42ms</tspan>
        <tspan fill="#C9D1D9"> | Uptime: </tspan>
        <tspan fill="#2EA043" font-weight="700">99.99%</tspan>
      </text>
    </g>

    <!-- Step 7: Active Prompt with Blinking Cursor -->
    <g class="line7">
      <text x="0" y="324">
        <tspan fill="#E63946" font-weight="700">root@p3rm4</tspan><tspan fill="#8B949E">:</tspan><tspan fill="#58A6FF">~/systems</tspan><tspan fill="#F1FAEE"> $ ./keep_shipping --mode=ultra-instinct</tspan>
      </text>
      <rect x="468" y="311" width="9" height="15" fill="#E63946" class="cursor" />
    </g>

  </g>

  <!-- ================= RIGHT PANEL: SPINNING ULTRA INSTINCT REACTOR HUD ================= -->
  <g transform="translate(818, 200)">
    <!-- Outer HUD Ring (Slow Clockwise Rotation) -->
    <g>
      <circle cx="0" cy="0" r="112" fill="none" stroke="#8B0000" stroke-width="1.5" stroke-dasharray="18 8 4 8" />
      <circle cx="0" cy="0" r="122" fill="none" stroke="#E63946" stroke-width="0.8" stroke-dasharray="4 16" stroke-opacity="0.6" />
      <animateTransform attributeName="transform" type="rotate" from="0" to="360" dur="24s" repeatCount="indefinite" />
    </g>

    <!-- Middle Cyber Ring (Counter-Clockwise Rotation) -->
    <g>
      <circle cx="0" cy="0" r="88" fill="none" stroke="#E63946" stroke-width="2.5" stroke-dasharray="45 25 15 25" filter="url(#glow)" />
      <polygon points="0,-96 -6,-84 6,-84" fill="#00F5D4" />
      <polygon points="0,96 -6,84 6,84" fill="#E63946" />
      <animateTransform attributeName="transform" type="rotate" from="360" to="0" dur="12s" repeatCount="indefinite" />
    </g>

    <!-- Inner High-Speed Ring -->
    <g>
      <circle cx="0" cy="0" r="62" fill="none" stroke="#00F5D4" stroke-width="1.5" stroke-dasharray="22 18" stroke-opacity="0.85" />
      <animateTransform attributeName="transform" type="rotate" from="0" to="360" dur="6s" repeatCount="indefinite" />
    </g>

    <!-- Core Glowing Orb -->
    <circle cx="0" cy="0" r="42" fill="#18060A" stroke="#E63946" stroke-width="2" filter="url(#glow)">
      <animate attributeName="r" values="39;44;39" dur="2.4s" repeatCount="indefinite" />
    </circle>

    <!-- Center Core Text -->
    <text x="0" y="-4" class="mono" font-size="14" font-weight="800" fill="#FFFFFF" text-anchor="middle" letter-spacing="1.5">P3RM4</text>
    <text x="0" y="13" class="mono" font-size="9" font-weight="600" fill="#E63946" text-anchor="middle" letter-spacing="1">CORE v4.9</text>
  </g>

  <!-- Right Panel Top Label -->
  <text x="818" y="68" class="mono" font-size="11" font-weight="700" fill="#8B949E" text-anchor="middle" letter-spacing="2">
    NEURAL TELEMETRY HUD
  </text>

  <!-- Right Panel Bottom Telemetry Readouts -->
  <g transform="translate(665, 345)" class="mono" font-size="11">
    <rect x="0" y="0" width="145" height="48" rx="6" fill="#12070A" stroke="#30363D" stroke-width="1" />
    <text x="12" y="19" fill="#8B949E">POWER INDEX</text>
    <text x="12" y="37" fill="#E63946" font-weight="700" font-size="13">OVER 9000+</text>

    <rect x="160" y="0" width="145" height="48" rx="6" fill="#12070A" stroke="#30363D" stroke-width="1" />
    <text x="172" y="19" fill="#8B949E">EXECUTION MODE</text>
    <text x="172" y="37" fill="#00F5D4" font-weight="700" font-size="13">ULTRA INSTINCT</text>
  </g>
</svg>
