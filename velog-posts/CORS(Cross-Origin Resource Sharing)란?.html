<p>CORS(Cross-Origin Resource Sharing)를 이해하기 위해 한국어로 번역해보면, '교차 출처 자원 공유'입니다.
대충 다른 URL에서 어떤 서버 자원을 요청할 수 있는지를 정해주는 정책 같은데, 막 와닿지는 않습니다. 😫</p>
<p>그러니, 한 단어씩 분해해보겠습니다.</p>
<h2 id="origin출처">Origin(출처)?</h2>
<p>만약, <code>https://www.example.com/login</code>에서 로그인을 한다고 했을 때,
<code>https://api.server.com/auth/login</code>로 로그인 정보를 보낸다고 합시다.</p>
<p>위 주소로 로그인 요청을 보낼 때, 우리는 요청 헤더를 같이 보내게 됩니다.
이때, 요청 헤더는 다음과 같습니다.</p>
<pre><code>POST /auth/login HTTP/1.1
Host: api.server.com
Origin: https://example.com
User-Agent: Mozilla/5.0
Accept: application/json</code></pre><p>🧐 위의 예시에서 알 수 있듯, <code>Origin</code>은 어디에서 웹 콘텐츠로 접근했는지를 나타냅니다.</p>
<p><img alt="" src="https://velog.velcdn.com/images/wonny_0724/post/5972a077-1f89-447e-8003-e68c657ec141/image.png" />
<em>(Source: Toss Payments 개발자센터 문서)</em></p>
<p>구체적으로는, 웹에서 Origin은 접근한 URL의 프로토콜, 호스트(호스트 이름, 포트)로 정의됩니다.</p>
<h3 id="cross-origin교차-출처">Cross-Origin(교차-출처)</h3>
<p>이렇게 Origin을 이해하였으니, Cross-Origin(교차 출처)이 의미하는 '출처가 교차한다'라는 것이 무엇인지 자연스럽게 이해가 될 것입니다.
정리해보면, Cross-origin은 자원을 주고 받으려는 두 출처가 서로 다르다는 뜻입니다.</p>
<p>만약 프론트엔드가 3000번 포트를, 백엔드가 3001번 포트를 사용한다면
프론트엔드에서 백엔드로 보내는 API 요청 또한 Cross-Origin에 해당하게 됩니다.
이는 URL의  포트가 다르기 때문입니다. 👍</p>
<p>또한, <code>www.example.com</code>에서 <code>api.example.com</code>으로 요청을 보낼 때에도 Cross-Origin에 해당합니다. 이는 호스트 네임(도메인)이 다르기 때문입니다.
즉, 서브 도메인이 다르면 다른 도메인으로 인식합니다.
(⚠️엄밀하게는, 호스트 이름과 도메인 이름은 다릅니다. 이를 다룬 글은 추후에 업로드 하겠습니다.)</p>
<h2 id="정리하자면">정리하자면,</h2>
<p>CORS는 자신과 프로토콜 또는 호스트가 다른 출처로부터자원을 가져오는 것이 되어야겠지만, 그렇지 않습니다. 😠
왜냐하면 CORS는 일종의 메커니즘이기 때문입니다.</p>
<p>그래서 CORS의 정확한 정의는 다음과 같습니다.
<strong>브라우저가 자신과 프로토콜 또는 호스트가 다른 출처로부터 자원을 가져오는 것을 허용하도록 서버가 허가해주는 HTTP 헤더 기반 메커니즘</strong>입니다.
즉, 사용자가 브라우저 내에서 <code>https://example.com</code>라는 웹사이트를 열었고 웹사이트가 <code>https://server.com</code>에게 &quot;너희한테 있는 사진 하나만 쓸게.&quot;라고 요청을 보냈을 때 브라우저가 이를 읽을 수 있게 서버가 허가해주는 HTTP 헤더 기반 메커니즘입니다.</p>
<p>위 문장은 자칫 &quot;서버가 허가한다&quot;는 행위를 중심으로 볼 여지가 있습니다.🫢
그런데 사실 CORS는 브라우저의 보안 모델이기에, 서버가 아닌 브라우저를 중심으로 봐야합니다.</p>
<p>브라우저는 기본적으로 SOP(Same-Origin Policy, 동일 출처 정책)을 따르기에, 다른 출처에서 자원을 받아오면 이것을 차단합니다. 🥲
이 SOP 정책에 예외를 추가해주는 것이 CORS입니다.</p>
<p>즉, CORS라는 메커니즘으로 SOP 정책에 예외를 추가하여 다른 출처에서 자원을 받아오는 것을 허용하는 것입니다.
이러면 이제 CORS가 메커니즘이라는 것이 이해가 됩니다.</p>
<p>그래서 백엔드 개발을 하다보면, 혼자 Postman으로 테스트할 때는 잘 동작하던 코드가 프론트엔드와 연결되는 순간 CORS 에러가 발생하는 것을 볼 수 있습니다. 😭😭😭😭
(제가 그 문제를 마주쳐서 정리할 겸 블로그 글을 작성중이긴 해요...)</p>
<h2 id="cors의-동작-과정">CORS의 동작 과정</h2>
<h3 id="기본적인-cors-동작-과정">기본적인 CORS 동작 과정</h3>
<ol>
<li><strong>브라우저는 교차 출처 요청(Cross-Origin Request)를 보낼 때 자동으로 <code>Origin</code>헤더를 추가합니다.</strong></li>
</ol>
<p>이 헤더는 CORS 요청을 판단하는 필수 신호입니다.</p>
<p>하지만, POST/PUT 등 일부 요청은 비-CORS 상황(Same-Origin Request)에서도 출처를 나타내는 헤더가 추가되기에 <strong>Origin 존재 -&gt; 교차 출처 요청</strong>은 아닙니다.⚠️</p>
<ol start="2">
<li><strong>서버는 응답에서 다음 헤더들로 &quot; 이 요청들은 공유해도 된다&quot;고 알려줍니다.</strong></li>
</ol>
<pre><code>Access-Control-Allow-Origin: https://example.com</code></pre><p>위 헤더는 <code>https://example.com</code>에서는 응답이 공유 가능하다는 것을 나타냅니다.
만약 어느 사이트에서나 응답을 공유하도록 하고 싶다면, URL 대신 <code>*</code>을 사용합니다.</p>
<p>만약, 요청에 쿠키나 Authorization 등 credentials가 포함된 경우에는 <code>*</code> 사용이 제한되며,</p>
<pre><code>Access-Control-Allow-Credentials: true</code></pre><p>헤더가 필요합니다.</p>
<h3 id="복잡한-cors에서의-동작-과정">복잡한 CORS에서의 동작 과정</h3>
<p>하지만 만약 CORS가 복잡한 경우에는 예외적으로 CORS-preflight Request(CORS 사전 요청)을 먼저 보내게 됩니다. 🫨🫨🫨
(이때, CORS-preflight Request는 브라우저에 의해 자동으로 수행됩니다.)</p>
<h4 id="복잡한-cors">복잡한 CORS?</h4>
<p>여기서 복잡한 경우란 다음과 같습니다.</p>
<ul>
<li>Content-Type이 브라우저의 안전 목록(safelist)에 없을 때</li>
<li>브라우저의 안전 목록에 없는 커스텀 헤더를 사용할 때</li>
<li>GET/HEAD/POST 외의 메서드를 사용하여 요청을 보낼 때</li>
<li>credentials 포함 여부 조건을 충족 할 때.
즉, 복잡한 CORS 요청이란 <code>&lt;form&gt;</code>으로 실행될 수 없는 요청이거나 브라우저가 보안상 위험하다고 판단하는 요청입니다.</li>
</ul>
<h4 id="cors-사전-요청">CORS 사전 요청</h4>
<p>CORS 사전 요청이란, <strong>CORS 프로토콜을 서버가 이해할 수 있는지 확인하는 역할을 하는 CORS 요청</strong>입니다. 이 요청은 <code>OPTIONS</code> 메서드를 사용하여 동일 엔드포인트(예: <code>/api</code>)로 보내집지며, 다음 헤더를 포함합니다.</p>
<ul>
<li><code>Access-Control-Request-Method</code>: 동일한 자원에 대한 실제 CORS 요청이 어떤 HTTP 메서드를 사용할 수 있는지를 확인합니다.</li>
<li><code>Access-Control-Request-Headers</code>: 동일한 장원에 대한 실제 CORS 요청이 어떤 헤더를 사용할 수 있는 지를 확인합니다.</li>
</ul>
<p>이 중 두번째 <code>Access-Control-Request-Headers</code>는 커스텀 헤더를 사용할 때에만 포함됩니다.</p>
<p>CORS 사전 요청에 대한 서버의 응답은 헤더를 포함할 수 있습니다.</p>
<ul>
<li><code>Access-Control-Allow-Methods</code>: CORS 프로토콜을 위해 해당 URL이 지원하는 HTTP 메서드를 나타냅니다.</li>
<li><code>Access-Control-Allow-Headers</code>: CORS 프로토콜을 위해 해당 URL이 지원하는 헤더를 나타냅니다.</li>
<li><code>Access-Control-Max-Age</code>: 위 두가지 헤더의 정보를 캐시할 수 있는 시간을 나타냅니다. 단위는 초이며, 기본 값은 5입니다.</li>
</ul>
<p><strong>서버의 응답이 &quot;허가&quot;일 때, 브라우저가 Preflight에서 요청한 메서드/헤더가 있다면 이에 대응하는 응답헤더는 필수적으로 작성하여야합니다.</strong>
서버의 응답이 &quot;불허&quot;일 때는 모든 헤더를 보내지 않아도 됩니다.</p>
<p>또한, CORS 사전 요청에 대한 <strong>성공 응답은 200 또는 204와 같은 정상 상태 응답으로 제한</strong>됩니다. 상태 코드가 2xx가 아닌 응답은 성공적이지 않은 것으로 간주되며, 실제 요청으로 이어지지 않습니다.</p>
<p>이런 과정을 거쳐 CORS 사전 응답이 성공한다면, 브라우저가 실제 CORS 요청을 다시 보냅니다.</p>
<hr />
<p>오늘은 팀플하다가 백엔드 API를 프론트엔드에 연결했더니 갑자기 CORS 에러가 뜨길래
이것 뭐예요?????? 하면서 CORS에 대해 정리해보았습니다.</p>
<p>글 적으면서 참고한 문서들은 아래에 적어둘게용.</p>
<p>Reference.
<a href="https://docs.tosspayments.com/resources/glossary/cors#%EC%9B%B9%EC%9D%98-%EB%B0%9C%EB%8B%AC%EA%B3%BC-cors">https://docs.tosspayments.com/resources/glossary/cors#웹의-발달과-cors</a>
<a href="https://developer.mozilla.org/ko/docs/Web/HTTP/Guides/CORS">https://developer.mozilla.org/ko/docs/Web/HTTP/Guides/CORS</a>
<a href="https://developer.mozilla.org/ko/docs/Glossary/Origin">https://developer.mozilla.org/ko/docs/Glossary/Origin</a>
<a href="https://fetch.spec.whatwg.org/#http-cors-protocol">https://fetch.spec.whatwg.org/#http-cors-protocol</a>
<a href="https://aws.amazon.com/ko/what-is/cross-origin-resource-sharing/">https://aws.amazon.com/ko/what-is/cross-origin-resource-sharing/</a></p>