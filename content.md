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
    Crypto Quant Researcher &amp; HFT Systems Engineer · Seoul 🇰🇷<br>
    Rust·Julia로 멀티 거래소 실시간 데이터 → 마켓 마이크로구조 모델링 → 주문 실행까지
    수직 통합한 트레이딩 시스템을 직접 설계합니다. 빗썸 수수료 0bp 기간 누적 거래대금 10억원+.
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

<h2 id="projects">🗂️ Projects</h2>

<div class="projects">

  <article class="proj reveal">
    <div class="proj-meta"><span class="yr">2025 – 2026</span> · Rust <span class="badge feat">★ Featured</span><span class="badge priv">Private</span></div>
    <div class="proj-title">amuredo-OMS-v2</div>
    <p class="proj-desc">
      순수 Rust로 마이그레이션한 멀티 거래소 주문관리시스템(OMS).<br>
      OMS 자체가 Feeder → MatchingEngine → FeatureStore → Pricing → Strategy 단계로 구성된 파이프라인으로,
      실시간 데이터 수집부터 주문 실행까지 전부 구현했습니다. 
    </p>
    <div class="metrics">
      <span class="metric g">tick-to-trade p50 4.23µs (net 제외)</span>
    </div>
    <div class="bd-grid">
      <div class="bd"><h5><span class="n">01</span>Engine &amp; Pipeline</h5><ul>
        <li>Julia+Rust DLL → 순수 Rust 마이그레이션</li>
        <li>Feeder→MatchingEngine→FeatureStore→Pricing→Strategy</li>
        <li>zero-allocation, state machine, DoubleBuffer lock-free</li></ul></div>
      <div class="bd"><h5><span class="n">02</span>Multi-exchange Data</h5><ul>
        <li>5 거래소 피더연결</li>
        <li>Matching Engine, Feature Store 기반 queue dynamic/cross symbol/cross exchange 피처 생성</li></ul></div>
      <div class="bd"><h5><span class="n">03</span>ML Market Making</h5><ul>
        <li>ML 미시구조 시그널 → maker 호가</li>
        <li>cross-symbol·cross-exchange 리서치</li></ul></div>
      <div class="bd"><h5><span class="n">05</span>OrderManagement</h5><ul>
        <li>FSM기반 안정적인 주문 관리</li>
        <li>missed fill 감지, REST 검증 폴백</li></ul></div>
      <div class="bd"><h5><span class="n">06</span>VirtualExchange</h5><ul>
        <li>Latency/Queue 고려가능한 가상 거래소 구현</li></ul></div>
    </div>
    <div class="stack"><span class="t">Rust (Infra)</span><span class="t">Julia (EDA)</span></div>
  </article>

  <article class="proj reveal">
    <div class="proj-meta"><span class="yr">2026</span> · Quant Research</div>
    <div class="proj-title">Quant Research &amp; Forward Tests</div>
    <p class="proj-desc">
      data analysis->smoked backtest->forwardtest 워크플로우 구축.
    </p>
    <div class="sub">Market Microstructure</div>
    <p class="proj-desc" style="margin-top:0">오더북 큐 마이크로구조 리서치 + 분석<br>머신러닝기반 시그널로 메이커 호가 제출<br>cross-symbol · cross-exchange 시그널 리서치</p>
    <div class="sub">ML / 통계 분석</div>
    <p class="proj-desc" style="margin-top:0">Model 학습<br> Shap분석을 통한 모델 해석<br>tstat/HAC를 통한 p-value 해석</p>
    <div class="sub">Forward Test (실거래 검증)</div>
    <p class="proj-desc" style="margin-top:0">BTC 낙주매매<br> 국내거래소 WLD pair-reversion<br>자체 제작 가상거래소는 queue position·latency까지 모델링해 괴리를 최소화<br>현재 ML 미시구조 시그널 기반 MM 전략을 실시간 forward test 중.</p>
  </article>

  <article class="proj reveal">
    <div class="proj-meta"><span class="yr">2026</span> · Rust · Julia <span class="badge priv">Private</span></div>
    <div class="proj-title">Forward Test · VirtualExchange</div>
    <p class="proj-desc">
      Smoked Backtest의 문제점을 해결하기 위한 가상거래소 기반 포워드 테스트.<br>
      backtest=Smoked Data기반 체결가정 / forward=VirtualExchange(라이브 피드) / live 3단계 검증
    </p>
    <div class="metrics">
    </div>
    <div class="sub">가상거래소(SimExchange) 모델링</div>
    <p class="proj-desc" style="margin-top:0">큐 포지션 추적 fill 모델 사다리(EndOfQueue→QueueBased) — 내 호가 앞 물량이 빠진 만큼만 체결.<br>레이턴시(주문 왕복·피드 지연)를 주입해 의사결정-체결 시차를 재현.</p>
    <div class="stack"><span class="t">Rust</span><span class="t">Julia</span><span class="t">SimExchange</span></div>
  </article>

  <article class="proj reveal">
    <div class="proj-meta"><span class="yr">2026</span> · Julia · Python <span class="badge priv">Private</span></div>
    <div class="proj-title">amuredo-alphafactor</div>
    <p class="proj-desc">
      크립토 선물 알파 리서치 플랫폼.<br>
      현재 주력은 Human-in-the-Loop 모드 — 터미널에서 Claude와 대화하며 Julia 데이터 서버(641 코인 × 227K 5분봉)에 실험을 직접 던지고,<br>
      실험 설계 → Julia 스크립트 → 결과 해석 루프를 빠르게 돕니다.<br> 
      장기적으로 HFT 플랫폼의 의사결정에 주입될 예정.
    </p>
    <div class="metrics">
      <span class="metric">641 symbols × 227K bars</span>
      <span class="metric g">vol-bar engine ~3× faster</span>
      <span class="metric">walk-forward 6-window OOS</span>
    </div>
    <div class="sub">거래량바(volume-bar) 엔진</div>
    <p class="proj-desc" style="margin-top:0">Volume Bar기반 리서치</p>
    <div class="sub">Pump-detect 전략</div>
    <div class="sub">리서치 factor</div>
    <p class="proj-desc" style="margin-top:0">premium(basis·김프) · open interest · funding rate · return momentum · volume · vwap · price-OI momentum.</p>
    <div class="sub">Long-Short 라이브 테스트</div>
    <div class="stack"><span class="t">Julia</span><span class="t">Python</span><span class="t">Claude Code (HITL)</span></div>
  </article>

  <article class="proj reveal">
    <div class="proj-meta"><span class="yr">2026</span> · Python · LLM <span class="badge live">● Live</span></div>
    <div class="proj-title">StoryQuant</div>
    <p class="proj-desc">
      뉴스 기반 한국 주식 인텔리전스 앱.<br>
      LLM(gpt-4o-mini)으로 헤드라인을 분류·노이즈 필터링하고, 그래프 RAG로 가격 변동의 사후 인과(attribution)를 추적합니다.<br>
      정직한 검증 — 예측이 아니라 70~90% 노이즈를 걸러내는 것이 목표.
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
      공급망 교란 하 동적 FJSSP 스케줄링을 위한 LLM 디스패칭-규칙 진화 연구 플랫폼.<br>
      논문 5편(AlphaEvolve·EoH·FunSearch·SeEvo·ReasoningBank)을 정리·구현하고, 6-mode RAG ablation으로 "failure-only 경험이 낫다"는 가설을 재현.<br>
      Rust DES 시뮬레이터 + 마법사 대시보드.
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
</div>

<h2 id="engineering">🛠️ Engineering &amp; Troubleshooting</h2>

<p class="ts-intro">amuredo-OMS(Julia+Rust)와 amuredo-OMS-v2(순수 Rust)를 만들며 부딪힌 실전 엔지니어링 고민과 해결의 기록</p>

<div class="ts-list">

  <article class="ts reveal">
    <div class="ts-h"><span class="n">02</span><span class="tt">피더 &amp; 피처 스토어</span><span class="en">feeder · FeatureStore</span></div>
    <p class="jp prob"><span class="lab">문제</span> 초당 수만 메시지를 받아<br>수십~수백 피처를 GC·락 없이 실시간 계산하려면?</p>
    <p class="jp sol"><span class="lab">해결</span> 피더(WS producer) → MatchingEngine → Channel 경쟁 소비.<br>오브젝트 풀(<code>get_from_pool!</code>/<code>release_to_pool!</code>)·<code>StaticRingBuffer</code>로 heap 할당 0.<br>FeatureStore는 3계층(Online/Offline/Cross)이고, 피처가 다른 피처를 구독(<code>use_*_feature_name</code>)하는 의존성 DAG 구조라 새 피처를 선언만으로 쉽게 추가.<br>틱마다 갱신되는 실시간(Online) 피처와 1초 주기로 갱신되는(Offline) 피처를 분리해 연산 부하를 적절히 배분.<br><code>ColumnStore</code> row-major f64 zero-copy, EMA 윈도우(갭 시 0 감쇠), HeartBeat가 1초 끊긴 피드 감지.<br>프로덕션 FeatureStoreSession×4·FeedSession×4 병렬.</p>
    <div class="metrics">
      <span class="metric g">DAG 피처 의존성</span>
      <span class="metric">realtime ↔ 1s 분리</span>
      <span class="metric">online 99 features</span>
      <span class="metric g">GC-zero pool</span>
    </div>
  </article>

  <article class="ts reveal">
    <div class="ts-h"><span class="n">03</span><span class="tt">모델 레이어</span><span class="en">PricingSession · DoubleBuffer</span></div>
    <p class="jp prob"><span class="lab">문제</span> 한 전략이 수십~99개 피처를 읽고 여러 모델을 µs 단위로 추론해야 한다.</p>
    <p class="jp sol"><span class="lab">해결</span> PricingSession이 <code>DoubleBuffer</code>(dirty-index만 복사, lock-free)로 피처를 공급.<br> <code>ctx.feature()</code>·<code>ctx.model()</code>·<code>ctx.feature_for(uid,name)</code> 읽기 전용 API만.<br>한 전략에 여러 모델(<code>HashMap&lt;String,Model&gt;</code>)을 등록해 µs 단위로 병렬 추론.</p>
    <div class="metrics">
      <span class="metric g">5 models feed→order p50 5.8µs</span>
      <span class="metric g">10 models 7–11µs</span>
      <span class="metric">read-only ctx API</span>
    </div>
  </article>

  <article class="ts reveal">
    <div class="ts-h"><span class="n">04</span><span class="tt">주문 제출</span><span class="en">order channel · state machine</span></div>
    <p class="jp prob"><span class="lab">문제</span> 전략 결정 → 거래소 REST까지,<br>핫패스에서 할당 없이 주문 수명을 안전하게 관리하려면?</p>
    <p class="jp sol"><span class="lab">해결</span> 주문은 order Channel(Strategy→OMS)로 흘러 REST 워커가 제출.<br>상태머신(<code>PlaceCreated→PlaceInFlight→Placed→Partial/Filled</code>, <code>CancelInFlight→Canceled</code>, <code>MaybeMissed</code>)<br>— 정의되지 않은 전이는 identity로 중복 이벤트를 흡수.<br>local↔exchange ID 양방향 매핑, zero-alloc 오브젝트 풀</p>
    <div class="metrics">
      <span class="metric">11-state FSM</span>
      <span class="metric g">zero-alloc OrderInOMS Pool</span>
      <span class="metric">local id↔exchange id map</span>
    </div>
  </article>

  <article class="ts reveal">
    <div class="ts-h"><span class="n">05</span><span class="tt">주문 경합</span><span class="en">contention · validation</span></div>
    <p class="jp prob"><span class="lab">문제</span> 취소가 체결과 동시에 날아오거나,<br>아직 ack 안 된 주문을 취소하거나, 같은 가격에 두 번 주문하면?</p>
    <p class="jp sol"><span class="lab">해결</span> 주문 제출 전 8가지 검증(<code>validation.rs</code>)<br>— cancel-while-canceling, SMP(자가체결 방지), duplicate-price, cancel-not-live, min qty/notional, NaN guard.<br><code>canceling_local_id_set</code>·<code>CancelInFlight</code>로 진행 중 취소를 추적하고,<br>stale-cancel sweep가 30s+ 멈춘 취소를 강제 종료해 지갑 예약금 잠김을 해제.<br>throttle·cancel-replace 케이던스(250ms·1Hz·10Hz).</p>
    <div class="metrics">
      <span class="metric">8 validation checks</span>
      <span class="metric">SMP · dup-price guard</span>
      <span class="metric g">stale-cancel sweep</span>
    </div>
  </article>

  <article class="ts reveal">
    <div class="ts-h"><span class="n">06</span><span class="tt">웹소켓 유저스트림</span><span class="en">user-stream · out-of-order · gap</span></div>
    <p class="jp prob"><span class="lab">문제</span> 거래소 WS가 체결을 호가 등록보다 먼저 보내거나,<br>이벤트를 빠뜨리거나(gap), 같은 체결을 두 번 보내면?</p>
    <p class="jp sol"><span class="lab">해결</span> ① 순서 역전 — <code>pending_ws_buffer</code>(64)가 early-fill을 버퍼링했다가 REST 매핑이 생기면 순서대로 replay.<br>② 누락 — <code>MissedFillDetector</code>가 체결틱이 내 호가를 관통하면 grace 2000ms 대기 후 REST로 실체 확인.<br>③ 끊김 — listen-key <code>keep_alive_loop</code> + 2–5s 백오프 auto-reconnect.<br>④ 중복 — <code>processed_trade_id_set</code> trade_id dedup + 상태머신 중복 흡수.</p>
    <div class="metrics">
      <span class="metric">early-fill replay buf 64</span>
      <span class="metric">missed-fill grace 2000ms</span>
      <span class="metric g">trade_id dedup</span>
    </div>
  </article>

</div>

<h2 id="journey">🧭 The Journey</h2>

데이터 분석으로 출발해 **강화학습에서 트레이딩에 빠진** 뒤, 매 단계마다 한계에 부딪히고 그걸 풀려고 다음 도구로 옮겨간 궤적입니다.<br>예측 → 의사결정 → 실행, Python → Julia → Rust.

<div class="journey">

  <div class="jnode reveal">
    <div class="jcard">
      <div class="jyear">2022 – 2023</div>
      <div class="jhead">AI · 데이터 분석</div>
      <p class="jp prob"><span class="lab">문제</span> 데이터에서 어떻게 의미 있는 패턴을 뽑아낼까?</p>
      <p class="jp sol"><span class="lab">해결</span> 머신러닝·통계·EDA로 데이터 분석에 입문<br>— 여러 도메인 데이터를 다루며 기초 체력을 쌓음.</p>
      <div class="jtags">machine-learning · mini-project · ML/DL 기초</div>
    </div>
  </div>

  <div class="jnode reveal">
    <div class="jcard">
      <div class="jyear">2023 – 2024</div>
      <div class="jhead">강화학습 — 트레이딩에 빠지다</div>
      <p class="jp prob"><span class="lab">문제</span> 지도학습은 단발 예측일 뿐<br>— 사고·팔고·보유의 순차적 의사결정을 담지 못한다.</p>
      <p class="jp sol"><span class="lab">해결</span> 여기서부터 트레이딩에 본격적으로 빠짐.<br>확률적(stochastic) 환경에서의 베팅·최적화 그 자체가 즐거웠던 게 계기.<br>매매를 순차 의사결정 문제로 보고 RL로 접근<br>— 커스텀 차트 환경·스캘핑 에이전트, 연구실에서 조합최적화 RL(TSP·VRP).</p>
      <div class="jtags">Reinforce-Learning · crypto-scalping-RL · Gym-Trading-Env · KHU AIMS LAB</div>
    </div>
  </div>

  <div class="jnode reveal">
    <div class="jcard">
      <div class="jyear">2024</div>
      <div class="jhead">마켓 마이크로구조 · HFT</div>
      <p class="jp prob"><span class="lab">문제</span> RL 백테스트가 실제 체결·호가창 동역학을 무시<br>→ 시뮬과 실거래의 괴리.</p>
      <p class="jp sol"><span class="lab">해결</span> 오더북을 직접 모델링<br>— LOB 딥러닝, online estimation, 고빈도 리서치.<br>Jane Street(Kaggle Bronze 🥉).</p>
      <p class="jp now"><span class="lab">+Rust</span> 이 무렵 Rust에 입문<br>— 『The Rust Programming Language』를 소유권·스마트 포인터까지 완독.<br>훗날 OMS Rust 재작성의 씨앗.</p>
      <div class="jtags">lob-deep-learning · deepOBs · online_estimation · ML-HFT · Hello-RUST-World</div>
    </div>
  </div>

  <div class="jnode reveal">
    <div class="jcard">
      <div class="jyear">2025</div>
      <div class="jhead">Julia 알파 리서치</div>
      <p class="jp prob"><span class="lab">문제</span> Python은 연구는 빠르지만 대규모 백테스트·실시간 연산이 느리다.</p>
      <p class="jp sol"><span class="lab">해결</span> Julia로 알파 리서치·백테스트 파이프라인 구축.<br><code>@view</code>·<code>@inbounds</code>·pre-alloc로 GC 최소화, 멀티스레딩 병렬화.</p>
      <div class="jtags">amuredo-EDA · amuredo-alphago · amuredo-StrategyStore</div>
    </div>
  </div>

  <div class="jnode reveal">
    <div class="jcard">
      <div class="jyear">2025</div>
      <div class="jhead">Julia OMS — 온몸 비틀기 최적화</div>
      <p class="jp prob"><span class="lab">문제</span> 리서치를 실거래로. GC가 있는 Julia로 마이크로초 핫패스를 버틸 수 있나?</p>
      <p class="jp sol"><span class="lab">해결</span> Julia로 OMS를 직접 구현하고 성능을 극한까지 짜냄:</p>
      <ul style="list-style:none">
        <li class="jopt">핫패스 전용 자료구조 직접 설계 — <code>DoubleBuffer</code>·<code>IdxSet</code>(dirty index)·<code>EfficientDict</code>·<code>MultipleBuffering</code> 링버퍼·hot-connection 풀(<code>OnePool</code>)</li>
        <li class="jopt">lock 경합 최소화 — <code>Channel</code> producer/consumer로 피처 생산↔소비 분리, 단일 상태는 <code>Atomic</code>으로 락 자체를 제거</li>
        <li class="jopt">Pricing 더블버퍼 — 쓰기는 back buffer, 읽기는 <code>Atomic</code> active-index 스냅샷이라 전략은 락 없이 read. <code>reconcile_dirty!</code>가 바뀐 인덱스만 복사</li>
        <li class="jopt"><code>@view</code> zero-copy 슬라이싱 · <code>@inbounds</code> 경계검사 제거</li>
        <li class="jopt">pre-allocation + in-place(<code>!</code>) 버퍼 재사용 → heap allocation 극한 감소</li>
        <li class="jopt">type stability(<code>@code_warntype</code>), 핫루프 박싱·동적 디스패치 제거</li>
        <li class="jopt"><code>Threads.@threads</code>·<code>@spawn</code> 병렬 연산 파이프라인</li>
        <li class="jopt">Julia 패키지·성능 한계는 <code>ccall</code> Rust DLL로 우회 (하이브리드)</li>
      </ul>
      <div class="jtags">Julia OMS · DoubleBuffer dirty-index · ccall FFI · Rust DLL hotpath</div>
    </div>
  </div>

  <div class="jnode cur reveal">
    <div class="jcard">
      <div class="jyear">2026 · 현재</div>
      <div class="jhead">순수 Rust OMS 🦀</div>
      <p class="jp prob"><span class="lab">문제</span> 온몸을 비틀어도 FFI 경계 오버헤드 + Julia GC 압박이 레이턴시·안정성의 병목.</p>
      <p class="jp sol"><span class="lab">해결</span> OMS 전면을 순수 Rust로 마이그레이션.<br>zero-alloc 상태머신, 11개 거래소 통합<br>→ tick-to-trade p50 4.23µs · 218K tps <span style="color:var(--dim)">(네트워크 제외, 내부 처리 기준)</span>.</p>
      <p class="jp now"><span class="lab">진행중</span> 2026년 1월부터 Claude Code(AI 에이전트)로 개발 가속<br>— 현재도 활발히 진행 중.</p>
      <div class="jtags">amuredo-OMS-v2 (Rust) · 102 commits / 2026</div>
    </div>
  </div>

</div>

<h2 id="archive">📦 Archive</h2>

예전에 적극적으로 파고든 AI/ML · HFT 리서치 — 지금의 작업으로 이어진 토대.

<div class="arch">
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
