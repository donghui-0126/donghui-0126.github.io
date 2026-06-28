<!--
  이 파일이 사이트 본문입니다. 여기를 고쳐서 커밋하면 사이트가 바로 바뀝니다.
  - 일반 글/목록/표/링크는 마크다운으로 자유롭게 수정하세요.
  - Journey / Projects / Engineering 같은 카드는 아래 <section> ... </section> HTML 블록을 그대로 두고 그 안의 글자만 고치면 됩니다.
  - 섹션 제목 <h2 id="..."> 의 id 는 상단 메뉴(앵커) 와 연결되니 바꾸지 마세요.
-->

<header class="profile" id="top">
  <div class="phead">
    <img class="avatar" src="https://github.com/donghui-0126.png" alt="Donghui Lim" loading="lazy" />
    <div>
      <div class="pname">Donghui Lim <span class="kr">임동휘</span></div>
      <div class="phandle">@donghui-0126</div>
    </div>
  </div>
  <p class="pbio">
    <b>Crypto Quant Researcher &amp; HFT Systems Engineer</b> · Seoul 🇰🇷<br>
    Rust·Julia로 멀티 거래소 실시간 데이터 → 마켓 마이크로구조 모델링 → 주문 실행까지
    수직 통합한 트레이딩 시스템을 직접 설계합니다. 빗썸 수수료 0bp 기간 <b>누적 거래대금 10억원+</b>.
  </p>
  <div class="plinks">
    <a class="plink solid" href="https://github.com/donghui-0126" target="_blank" rel="noopener">GitHub ↗</a>
    <a class="plink" href="mailto:lukedonghui@gmail.com">✉ Email</a>
    <a class="plink" href="https://donghui-0126.github.io/StoryQuant/" target="_blank" rel="noopener">StoryQuant Demo ↗</a>
  </div>
</header>

<h2 id="interest">🔬 Interest</h2>

<div class="tags">
  <span class="chip">HFT</span>
  <span class="chip">Market Microstructure</span>
  <span class="chip">Market Making</span>
  <span class="chip">Alpha Research</span>
  <span class="chip">AI</span>
  <span class="chip">Low-latency Systems · Rust</span>
  <span class="chip">LLM Research Infra</span>
</div>

<h2 id="education">🎓 Education</h2>

**경희대학교 산업경영공학과** · *Kyung Hee University, Industrial &amp; Management Systems Engineering* — 학부 재학 중 · 2027 졸업예정

<h2 id="journey">🧭 The Journey</h2>

데이터 분석으로 출발해 **강화학습에서 트레이딩에 빠진** 뒤, 매 단계마다 한계에 부딪히고 그걸 풀려고 다음 도구로 옮겨간 궤적입니다. 예측 → 의사결정 → 실행, Python → Julia → Rust.

<div class="journey">

  <div class="jnode reveal">
    <div class="jcard">
      <div class="jyear">2022 – 2023</div>
      <div class="jhead">AI · 데이터 분석</div>
      <p class="jp prob"><span class="lab">문제</span> 데이터에서 어떻게 <b>의미 있는 패턴</b>을 뽑아낼까?</p>
      <p class="jp sol"><span class="lab">해결</span> 머신러닝·통계·EDA로 데이터 분석에 입문 — 여러 도메인 데이터를 다루며 기초 체력을 쌓음.</p>
      <div class="jtags">machine-learning · mini-project · ML/DL 기초</div>
    </div>
  </div>

  <div class="jnode reveal">
    <div class="jcard">
      <div class="jyear">2023 – 2024</div>
      <div class="jhead">강화학습 — 트레이딩에 빠지다</div>
      <p class="jp prob"><span class="lab">문제</span> 지도학습은 <b>단발 예측</b>일 뿐 — 사고·팔고·보유의 순차적 의사결정을 담지 못한다.</p>
      <p class="jp sol"><span class="lab">해결</span> 여기서부터 트레이딩에 본격적으로 빠짐. <b>확률적(stochastic) 환경에서의 베팅·최적화 그 자체가 즐거웠던 게 계기</b>. 매매를 <b>순차 의사결정 문제</b>로 보고 RL로 접근 — 커스텀 차트 환경·스캘핑 에이전트, 연구실에서 조합최적화 RL(TSP·VRP).</p>
      <div class="jtags">Reinforce-Learning · crypto-scalping-RL · Gym-Trading-Env · KHU AIMS LAB</div>
    </div>
  </div>

  <div class="jnode reveal">
    <div class="jcard">
      <div class="jyear">2024</div>
      <div class="jhead">마켓 마이크로구조 · HFT</div>
      <p class="jp prob"><span class="lab">문제</span> RL 백테스트가 실제 <b>체결·호가창 동역학</b>을 무시 → 시뮬과 실거래의 괴리.</p>
      <p class="jp sol"><span class="lab">해결</span> 오더북을 직접 모델링 — LOB 딥러닝, online estimation, 고빈도 리서치. Jane Street(Kaggle Bronze 🥉).</p>
      <p class="jp now"><span class="lab">+Rust</span> 이 무렵 <b>Rust에 입문</b> — 『The Rust Programming Language』를 소유권·스마트 포인터까지 완독. 훗날 OMS Rust 재작성의 씨앗.</p>
      <div class="jtags">lob-deep-learning · deepOBs · online_estimation · ML-HFT · Hello-RUST-World</div>
    </div>
  </div>

  <div class="jnode reveal">
    <div class="jcard">
      <div class="jyear">2025</div>
      <div class="jhead">Julia 알파 리서치</div>
      <p class="jp prob"><span class="lab">문제</span> Python은 연구는 빠르지만 <b>대규모 백테스트·실시간 연산이 느리다.</b></p>
      <p class="jp sol"><span class="lab">해결</span> Julia로 알파 리서치·백테스트 파이프라인 구축. <code>@view</code>·<code>@inbounds</code>·pre-alloc로 GC 최소화, 멀티스레딩 병렬화.</p>
      <div class="jtags">amuredo-EDA · amuredo-alphago · amuredo-StrategyStore</div>
    </div>
  </div>

  <div class="jnode reveal">
    <div class="jcard">
      <div class="jyear">2025</div>
      <div class="jhead">Julia OMS — 온몸 비틀기 최적화</div>
      <p class="jp prob"><span class="lab">문제</span> 리서치를 실거래로. GC가 있는 Julia로 <b>마이크로초 핫패스</b>를 버틸 수 있나?</p>
      <p class="jp sol"><span class="lab">해결</span> Julia로 OMS를 직접 구현하고 성능을 <b>극한까지 짜냄</b>:</p>
      <ul style="list-style:none">
        <li class="jopt"><b>핫패스 전용 자료구조 직접 설계</b> — <code>DoubleBuffer</code>·<code>IdxSet</code>(dirty index)·<code>EfficientDict</code>·<code>MultipleBuffering</code> 링버퍼·hot-connection 풀(<code>OnePool</code>)</li>
        <li class="jopt"><b>lock 경합 최소화</b> — <code>Channel</code> producer/consumer로 피처 생산↔소비 분리, 단일 상태는 <code>Atomic</code>으로 락 자체를 제거</li>
        <li class="jopt"><b>Pricing 더블버퍼</b> — 쓰기는 back buffer, 읽기는 <code>Atomic</code> active-index 스냅샷이라 전략은 <b>락 없이 read</b>. <code>reconcile_dirty!</code>가 <b>바뀐 인덱스만</b> 복사</li>
        <li class="jopt"><code>@view</code> zero-copy 슬라이싱 · <code>@inbounds</code> 경계검사 제거</li>
        <li class="jopt">pre-allocation + in-place(<code>!</code>) 버퍼 재사용 → <b>heap allocation 극한 감소</b></li>
        <li class="jopt">type stability(<code>@code_warntype</code>), 핫루프 박싱·동적 디스패치 제거</li>
        <li class="jopt"><code>Threads.@threads</code>·<code>@spawn</code> 병렬 연산 파이프라인</li>
        <li class="jopt">Julia 패키지·성능 한계는 <code>ccall</code> <b>Rust DLL</b>로 우회 (하이브리드)</li>
      </ul>
      <div class="jtags">Julia OMS · DoubleBuffer dirty-index · ccall FFI · Rust DLL hotpath</div>
    </div>
  </div>

  <div class="jnode cur reveal">
    <div class="jcard">
      <div class="jyear">2026 · 현재</div>
      <div class="jhead">순수 Rust OMS 🦀</div>
      <p class="jp prob"><span class="lab">문제</span> 온몸을 비틀어도 FFI 경계 오버헤드 + Julia <b>GC 압박</b>이 레이턴시·안정성의 병목.</p>
      <p class="jp sol"><span class="lab">해결</span> OMS 전면을 <b>순수 Rust로 마이그레이션</b>. zero-alloc 상태머신, 11개 거래소 통합 → <b>tick-to-trade p50 4.23µs · 218K tps</b>.</p>
      <p class="jp now"><span class="lab">진행중</span> <b>2026년 1월</b>부터 Claude Code(AI 에이전트)로 개발 가속 — 현재도 활발히 진행 중.</p>
      <div class="jtags">amuredo-OMS-v2 (Rust) · 102 commits / 2026</div>
    </div>
  </div>

</div>

<h2 id="projects">🗂️ Projects</h2>

<div class="projects">

  <article class="proj reveal">
    <div class="proj-meta"><span class="yr">2025 – 2026</span> · Rust <span class="badge feat">★ Featured</span><span class="badge priv">Private</span></div>
    <div class="proj-title">amuredo-OMS-v2</div>
    <p class="proj-desc">
      순수 <b>Rust</b>로 마이그레이션한 멀티 거래소 주문관리시스템(OMS). 실시간 데이터 수집부터 주문 실행까지
      수직 통합했고, <b>2026년 102개 커밋</b>에 걸쳐 직접 설계·구현했습니다.
    </p>
    <div class="metrics">
      <span class="metric g">tick-to-trade p50 4.23µs</span>
      <span class="metric g">218K tps</span>
      <span class="metric">27 crates</span>
      <span class="metric">11 exchanges</span>
      <span class="metric">CPU −27%</span>
    </div>
    <div class="bd-grid">
      <div class="bd"><h5><span class="n">01</span>Engine &amp; Pipeline</h5><ul>
        <li>Julia+Rust DLL → <b>순수 Rust 마이그레이션</b></li>
        <li>Feeder→Matching→FeatureStore→Pricing→OMS</li>
        <li>zero-alloc 상태머신, <code>DoubleBuffer</code> lock-free</li></ul></div>
      <div class="bd"><h5><span class="n">02</span>Multi-exchange Data</h5><ul>
        <li>11거래소 인증(<code>JWT</code>·<code>HMAC</code>)</li>
        <li>Binance 선물 <b>577종목</b> + watchdog</li>
        <li>BTreeMap depth book → CPU −27%</li></ul></div>
      <div class="bd"><h5><span class="n">03</span>Latency / Parsing</h5><ul>
        <li>크기 기반 JSON 파싱 라우팅 8거래소</li>
        <li>wire-to-order·multi-feeder 벤치마크</li>
        <li><code>PARSING_LATENCY_SPEC</code> 명세화</li></ul></div>
      <div class="bd"><h5><span class="n">04</span>ML Market Making</h5><ul>
        <li>ML <b>미시구조 시그널</b> → maker 호가</li>
        <li>97-feature 스키마 + 모델 로더</li>
        <li>cross-symbol·cross-exchange 리서치</li></ul></div>
      <div class="bd"><h5><span class="n">05</span>Execution Safety</h5><ul>
        <li>missed fill 감지, REST 검증 폴백</li>
        <li>graceful flatten, Stop/Shutdown API</li>
        <li>실시간 forward-test 대시보드</li></ul></div>
      <div class="bd"><h5><span class="n">06</span>Quality &amp; Docs</h5><ul>
        <li><b>4-pass 감사</b> — 22건 수정</li>
        <li>계층형 <code>AGENTS.md</code>, MODEL_REGISTRY</li>
        <li>Strategy Playbook (15 전략 예시)</li></ul></div>
    </div>
    <div class="stack"><span class="t">Rust</span><span class="t">tokio</span><span class="t">simd-json</span><span class="t">Polars/Parquet</span><span class="t">Julia (models)</span></div>
  </article>

  <article class="proj reveal">
    <div class="proj-meta"><span class="yr">2026</span> · Python · LLM <span class="badge live">● Live</span></div>
    <div class="proj-title">StoryQuant</div>
    <p class="proj-desc">
      뉴스 기반 한국 주식 인텔리전스 앱. <b>LLM(gpt-4o-mini)</b>으로 헤드라인을 분류·노이즈 필터링하고,
      그래프 RAG로 가격 변동의 사후 인과(attribution)를 추적합니다.
      <b>정직한 검증 — 예측이 아니라 70~90% 노이즈를 걸러내는 것</b>이 목표.
    </p>
    <div class="metrics">
      <span class="metric">RAG</span>
      <span class="metric">검색 8–10s → ~2s</span>
      <span class="metric">Supabase · Render 실배포</span>
    </div>
    <div class="stack"><span class="t">Python</span><span class="t">JS</span><span class="t">LLM</span><span class="t">Supabase</span></div>
    <div class="plinks-row">
      <a href="https://donghui-0126.github.io/StoryQuant/" target="_blank" rel="noopener">live demo ↗</a>
      <a href="https://github.com/donghui-0126/StoryQuant" target="_blank" rel="noopener">source ↗</a>
    </div>
  </article>

  <article class="proj reveal">
    <div class="proj-meta"><span class="yr">2026</span> · Python · Rust · LLM <span class="badge live">● Live</span></div>
    <div class="proj-title">heuristiX</div>
    <p class="proj-desc">
      공급망 교란 하 동적 FJSSP 스케줄링을 위한 <b>LLM 디스패칭-규칙 진화</b> 연구 플랫폼.
      논문 5편(AlphaEvolve·EoH·FunSearch·SeEvo·ReasoningBank)을 정리·구현하고,
      <b>6-mode RAG ablation</b>으로 "failure-only 경험이 낫다"는 가설을 재현. Rust DES 시뮬레이터 + 마법사 대시보드.
    </p>
    <div class="metrics">
      <span class="metric">EoH 4-operator 진화</span>
      <span class="metric">6-mode RAG ablation</span>
    </div>
    <div class="stack"><span class="t">Python</span><span class="t">Rust</span><span class="t">LLM</span><span class="t">Flask</span></div>
    <div class="plinks-row">
      <a href="https://heuristix.onrender.com" target="_blank" rel="noopener">live dashboard ↗</a>
      <a href="https://github.com/donghui-0126/heuristiX-v2" target="_blank" rel="noopener">source ↗</a>
    </div>
  </article>

  <article class="proj reveal">
    <div class="proj-meta"><span class="yr">2026</span> · Rust</div>
    <div class="proj-title">amure-do / amure-db</div>
    <p class="proj-desc">
      <b>Rust</b>로 직접 만든 그래프 RAG 지식 엔진. <b>amure-db</b>는 임베딩+그래프 하이브리드 3-layer 검색
      (cosine → graph walk → MMR), <b>amure-do</b>는 이를 도메인 불문 가설 기반 연구 엔진으로 일반화(11 LLM providers).
      레거시 38→15파일 클린 리빌드.
    </p>
    <div class="stack"><span class="t">Rust</span><span class="t">embeddings</span><span class="t">graph</span></div>
    <div class="plinks-row">
      <a href="https://github.com/donghui-0126/amure-do" target="_blank" rel="noopener">amure-do ↗</a>
      <a href="https://github.com/donghui-0126/amure-db" target="_blank" rel="noopener">amure-db ↗</a>
    </div>
  </article>

  <article class="proj reveal">
    <div class="proj-meta"><span class="yr">2026</span> · Julia · Rust · LLM <span class="badge priv">Private</span></div>
    <div class="proj-title">amuredo-alphafactor</div>
    <p class="proj-desc">
      크립토 선물 <b>알파 리서치 플랫폼</b>. 가설(hypothesis) 하나를 넣으면 <b>RAG → LLM 가설 생성 → Julia 배치 실험 → 해석 → accept/decline 판결 → 지식그래프 저장</b>까지 7단계를 자동화.
      Julia 서버가 <b>537개 코인 × 227K 바</b>를 들고 cross-sectional IC를 돌리고, 가설은 <b>amure-db 지식그래프</b>(subset/superset/reference 엣지·역방향 자동)로 축적합니다.
    </p>
    <div class="metrics">
      <span class="metric">537 symbols × 227K bars</span>
      <span class="metric">288 가설 / 6 팩터</span>
      <span class="metric">6 실험 (고정 3 + LLM-guided 3)</span>
    </div>
    <div class="sub">리서치한 팩터</div>
    <p class="proj-desc" style="margin-top:0">premium(basis·김프) · open interest · funding rate · return momentum · volume · vwap · price-OI momentum — Universe/Regime/Temporal cross-sectional IC로 검증.</p>
    <div class="sub">Long-Short 라이브 테스트 (사이드 프로젝트)</div>
    <p class="proj-desc" style="margin-top:0">검증된 <b>크로스섹셔널 롱숏 전략 4종</b>을 바이낸스 선물에 <b>실시간 forward 모니터링</b>(5분 REST 폴링·view-only) — quintile L/S · meme Top-50 · 12h hold.</p>
    <div class="stack"><span class="t">Julia</span><span class="t">Rust (amure-db)</span><span class="t">Python</span><span class="t">LLM</span></div>
  </article>

  <article class="proj reveal">
    <div class="proj-meta"><span class="yr">2024 – 2026</span> · Quant Research</div>
    <div class="proj-title">Quant Research &amp; Forward Tests</div>
    <p class="proj-desc">
      시스템 구축에서 끝내지 않고, 실제 데이터로 시그널을 검증하고 전략을 <b>forward test</b>까지 돌립니다.
    </p>
    <div class="sub">Market Microstructure</div>
    <p class="proj-desc" style="margin-top:0">오더북 <b>큐 마이크로구조</b> 리서치 + 분석 툴링 (빗썸). <b>머신러닝으로 미시구조 시그널(오더플로·큐 동역학)을 추출</b>해 fair-value·메이커 호가에 반영. <b>cross-symbol · cross-exchange</b> 시그널 리서치도 병행.</p>
    <div class="sub">ML / 통계 분석</div>
    <p class="proj-desc" style="margin-top:0"><b>fair-value 모델링</b>(walk-forward) · 팩터 분석 <code>IC · IR · hit ratio</code> · calibration.</p>
    <div class="sub">Forward Test (실거래 검증)</div>
    <p class="proj-desc" style="margin-top:0"><b>BTC 낙주매매</b>(급락 후 반등) · <b>WLD</b> pair-reversion · <b>국내 거래소 MM</b>(빗썸) · 모델 기반 MM. 자체 제작 <b>가상거래소는 큐 포지션(queue position)·레이턴시(latency)까지 모델링</b>해 sim↔실거래 괴리를 최소화했고, 현재 <b>ML 미시구조 시그널 기반 MM 전략을 실시간 forward test 중</b>.</p>
  </article>

</div>

<h2 id="engineering">🛠️ Engineering &amp; Troubleshooting</h2>

<p class="ts-intro"><b>amuredo-OMS</b>(Julia+Rust)와 <b>amuredo-OMS-v2</b>(순수 Rust)를 만들며 부딪힌 실전 엔지니어링 고민과 해결의 기록 — 데이터 수집부터 실거래 정합성까지 7개 단계. <span style="color:var(--dim)">알파·시그널 내용은 제외, 시스템 설계와 트러블슈팅만.</span></p>

<div class="ts-list">

  <article class="ts reveal">
    <div class="ts-h"><span class="n">01</span><span class="tt">데이터 수집</span><span class="en">data-save · parquet archival</span></div>
    <p class="jp prob"><span class="lab">문제</span> 멀티 거래소 원시 틱을 손실 없이 보관하면서, <b>수집 부하 자체가 데이터를 오염시키지 않게</b> 하려면?</p>
    <p class="jp sol"><span class="lab">해결</span> <b>3,349 심볼 × 12 거래소</b>를 시간단위 Parquet 파티션(<code>&lt;거래소&gt;/&lt;심볼&gt;/&lt;YYYYMMDD_HH&gt;</code>)으로 아카이빙, watchdog 싱글톤으로 단일 인스턴스 강제. 60k msg/sec 고부하에서 OS NIC batching이 <b>RX→consumer lag p99를 1,140ms</b>까지 밀어 1Hz 스냅샷이 stale해지는 "silent contamination"을 측정으로 발견 → 프로세스당 <b>≤50k msg/sec ≈ 800심볼</b> 안전선으로 분할.</p>
    <div class="metrics">
      <span class="metric">3,349 심볼 × 12 거래소</span>
      <span class="metric g">lag p99 1140ms → 95ms</span>
      <span class="metric">≤50k msg/sec / proc</span>
    </div>
  </article>

  <article class="ts reveal">
    <div class="ts-h"><span class="n">02</span><span class="tt">피더 &amp; 피처 스토어</span><span class="en">feeder · FeatureStore</span></div>
    <p class="jp prob"><span class="lab">문제</span> 초당 수만 메시지를 받아 <b>수십~수백 피처를 GC·락 없이</b> 실시간 계산하려면?</p>
    <p class="jp sol"><span class="lab">해결</span> 피더(WS producer) → MatchingEngine → Channel 경쟁 소비. 오브젝트 풀(<code>get_from_pool!</code>/<code>release_to_pool!</code>)·<code>StaticRingBuffer</code>로 <b>heap 할당 0</b>. FeatureStore는 3계층(Online/Offline/Cross), <code>ColumnStore</code> row-major f64 <b>zero-copy</b>, EMA 윈도우(갭 시 0 감쇠), <b>HeartBeat</b>가 1초 끊긴 피드 감지. 프로덕션 FeatureStoreSession×4·FeedSession×4 병렬.</p>
    <div class="metrics">
      <span class="metric">online 99 features</span>
      <span class="metric">Brief 22 · Tick 21 · OrderFlow 56</span>
      <span class="metric g">GC-zero pool</span>
    </div>
  </article>

  <article class="ts reveal">
    <div class="ts-h"><span class="n">03</span><span class="tt">모델 레이어</span><span class="en">PricingSession · DoubleBuffer</span></div>
    <p class="jp prob"><span class="lab">문제</span> 한 전략이 <b>수십~99개 피처를 읽고 여러 모델을 µs 단위로 추론</b>해야 한다. 전략이 피처를 직접 계산하면 sim↔live 정합성이 깨진다.</p>
    <p class="jp sol"><span class="lab">해결</span> PricingSession이 <code>DoubleBuffer</code>(dirty-index만 복사, lock-free)로 피처를 공급. 전략은 피처 계산 <b>금지</b> — <code>ctx.feature()</code>·<code>ctx.model()</code>·<code>ctx.feature_for(uid,name)</code> 읽기 전용 API만. 한 전략에 <b>여러 모델</b>(<code>HashMap&lt;String,Model&gt;</code>): RidgeOLS(static ~1µs) + OnlineRidge(매초 refit <code>β=(X'X+λI)⁻¹X'y</code>, rolling IC).</p>
    <div class="metrics">
      <span class="metric g">5 models feed→order p50 5.8µs</span>
      <span class="metric g">10 models 7–11µs</span>
      <span class="metric">read-only ctx API</span>
    </div>
  </article>

  <article class="ts reveal">
    <div class="ts-h"><span class="n">04</span><span class="tt">주문 제출</span><span class="en">order channel · state machine</span></div>
    <p class="jp prob"><span class="lab">문제</span> 전략 결정 → 거래소 REST까지, <b>핫패스에서 할당 없이</b> 주문 수명을 안전하게 관리하려면?</p>
    <p class="jp sol"><span class="lab">해결</span> 주문은 order Channel(Strategy→OMS)로 흘러 REST 워커가 제출. <b>상태머신</b>(<code>PlaceCreated→PlaceInFlight→Placed→Partial/Filled</code>, <code>CancelInFlight→Canceled</code>, <code>MaybeMissed</code>) — 정의되지 않은 전이는 identity로 <b>중복 이벤트를 흡수</b>. local↔exchange ID 양방향 매핑, <b>zero-alloc 오브젝트 풀</b>(v1 사전할당 50만 개).</p>
    <div class="metrics">
      <span class="metric">11-state FSM</span>
      <span class="metric g">zero-alloc OioPool</span>
      <span class="metric">local↔exchange id map</span>
    </div>
  </article>

  <article class="ts reveal">
    <div class="ts-h"><span class="n">05</span><span class="tt">주문 경합</span><span class="en">contention · validation</span></div>
    <p class="jp prob"><span class="lab">문제</span> 취소가 <b>체결과 동시에</b> 날아오거나, 아직 ack 안 된 주문을 취소하거나, 같은 가격에 두 번 주문하면?</p>
    <p class="jp sol"><span class="lab">해결</span> 배치 전 <b>8가지 검증</b>(<code>validation.rs</code>) — cancel-while-canceling, <b>SMP(자가체결 방지)</b>, duplicate-price, cancel-not-live, min qty/notional, NaN guard. <code>canceling_local_id_set</code>·<code>CancelInFlight</code>로 진행 중 취소를 추적하고, <b>stale-cancel sweep</b>가 30s+ 멈춘 취소를 강제 종료해 지갑 예약금 잠김을 해제. throttle·cancel-replace 케이던스(250ms·1Hz·10Hz).</p>
    <div class="metrics">
      <span class="metric">8 validation checks</span>
      <span class="metric">SMP · dup-price guard</span>
      <span class="metric g">stale-cancel sweep</span>
    </div>
  </article>

  <article class="ts reveal">
    <div class="ts-h"><span class="n">06</span><span class="tt">웹소켓 유저스트림</span><span class="en">user-stream · out-of-order · gap</span></div>
    <p class="jp prob"><span class="lab">문제</span> 거래소 WS가 <b>체결을 ACK보다 먼저</b> 보내거나, 이벤트를 빠뜨리거나(gap), 같은 체결을 두 번 보내면?</p>
    <p class="jp sol"><span class="lab">해결</span> ① <b>순서 역전</b> — <code>pending_ws_buffer</code>(64)가 early-fill을 버퍼링했다가 REST 매핑이 생기면 순서대로 replay. ② <b>누락</b> — <code>MissedFillDetector</code>가 체결틱이 내 호가를 관통하면 grace <b>2000ms</b> 대기 후 REST로 실체 확인. ③ <b>끊김</b> — listen-key <code>keep_alive_loop</code> + 2–5s 백오프 auto-reconnect. ④ <b>중복</b> — <code>processed_trade_id_set</code> trade_id dedup + 상태머신 중복 흡수.</p>
    <div class="metrics">
      <span class="metric">early-fill replay buf 64</span>
      <span class="metric">missed-fill grace 2000ms</span>
      <span class="metric g">trade_id dedup</span>
    </div>
  </article>

  <article class="ts reveal">
    <div class="ts-h"><span class="n">07</span><span class="tt">백테스트 → 포워드 → 실거래 정합성</span><span class="en">backtest · sim · live parity ⭐</span></div>
    <p class="jp prob"><span class="lab">문제</span> smoked 백테스트에서 좋던 전략이 <b>가상거래소 포워드 → 실거래</b>로 갈수록 무너진다. 어디서 새는지 어떻게 잡나?</p>
    <p class="jp sol"><span class="lab">해결</span> 3단계가 <b>같은 전략 바이너리</b>를 실행(backtest=MockExchange / forward=SimExchange 라이브 피드 / live). 시간 주입(<code>ctx.now_ms()</code>)으로 결정론 보장, fill 모델 사다리 EndOfQueue→QueueBased. 정합성은 <b>same-window 규칙</b> + yhat 분포 parity(<code>σ ratio∈[0.85,1.15]</code>, same-second <code>ρ≥0.85</code>) + <code>feat_hash</code> byte 일치로 검증.</p>
    <p class="jp res"><span class="lab">결과</span> Rust↔Julia 예측 <b>Pearson 1.000000</b>(max diff 7e-9) 달성. 백테스트 +18.8bp인데 같은 구간 실거래 −29¢(~5bp 낙관 갭, 큐 포지션 미모델링)를 정직하게 기록 → "Sim PnL 숫자 자체는 믿지 말고 same-window로만 비교", 배포 전 <b>8단계 체크리스트</b> 통과 규약.</p>
    <div class="metrics">
      <span class="metric g">Rust↔Julia Pearson 1.000000</span>
      <span class="metric">3-stage, same binary</span>
      <span class="metric">8-step deploy gate</span>
    </div>
  </article>

</div>

<h2 id="archive">📦 Archive</h2>

예전에 적극적으로 파고든 AI/ML · HFT 리서치 — 지금의 작업으로 이어진 토대.

<div class="arch">
  <a class="achip" href="https://github.com/donghui-0126/ML-HFT" target="_blank" rel="noopener">ML-HFT <span>· ML HFT framework</span></a>
  <a class="achip" href="https://github.com/donghui-0126/deepOBs" target="_blank" rel="noopener">deepOBs <span>· DL orderbook</span></a>
  <a class="achip" href="https://github.com/donghui-0126/lob-world-models" target="_blank" rel="noopener">lob-world-models <span>· model-based RL</span></a>
  <a class="achip" href="https://github.com/donghui-0126/lob-deep-learning" target="_blank" rel="noopener">lob-deep-learning <span>· LOB DL</span></a>
  <a class="achip" href="https://github.com/donghui-0126/online_estimation" target="_blank" rel="noopener">online_estimation</a>
  <a class="achip" href="https://github.com/donghui-0126/JaneStreetKaggle" target="_blank" rel="noopener">JaneStreetKaggle <span>· Bronze 🥉</span></a>
  <a class="achip" href="https://github.com/donghui-0126/Machine-Learning-for-Factor-Investing" target="_blank" rel="noopener">ML for Factor Investing</a>
  <a class="achip" href="https://github.com/donghui-0126/crypto-scalping-RL-Agent" target="_blank" rel="noopener">crypto-scalping-RL</a>
  <a class="achip" href="https://github.com/donghui-0126/Hello-RUST-World" target="_blank" rel="noopener">Hello-RUST-World <span>· Rust 입문</span></a>
</div>

<h2 id="awards">🏅 Awards &amp; Experience</h2>

| Year | Competition | Result |
|------|-------------|--------|
| 2025 | Jane Street — Real-Time Market Data Forecasting (Kaggle) | **Bronze 🥉** |
| 2024 | BDA × ASCEND — Bitcoin Volatility Prediction | **우수상** |
| 2023 | WorldQuant Alphaton Korea | **3rd 🥉** |
| 2023 | FSI Data Challenge — EV Customer Prediction | **우수상** |

> **Publication** · Hyeong-jin Son, **Lim Donghui**, & Young-woo Han (2023). *Reinforcement learning portfolio optimization based on portfolio theory.* 한국정보처리학회 학술대회논문집, 30(2), 961–962.

**Experience**

- **KHU AIMS LAB** · Undergraduate Researcher (2024) — Combinatorial Optimization with RL (TSP, VRP)
- **모두의연구소 PISTAR LAB** (2024) — Algorithm Trading with AI
- **KHUDA 3–4기** Financial Track (2023) · **금융공학 학회 UFEA** 36기
