hookJS is a very simple library that allows a developer to call "hooks", hooks being a nice way of organizing one to many anonymous functions as well as linking events to functions.
      
A great use case is a javascript video game controller where you have directional states.  Up, down, left, and right would all have hooks that would have functions attached to them.

Here is some example code...
<pre>
hook<span style='color:#d2cd86; '>.</span>add<span style='color:#d2cd86; '>(</span><span style='color:#00c4c4; '>'example'</span><span style='color:#d2cd86; '>,</span> <span style='color:#e66170; font-weight:bold; '>function</span> <span style='color:#d2cd86; '>(</span>foo<span style='color:#d2cd86; '>,</span> bar<span style='color:#d2cd86; '>)</span> <span style='color:#b060b0; '>{</span>
  console<span style='color:#d2cd86; '>.</span><span style='color:#e66170; font-weight:bold; '>log</span><span style='color:#d2cd86; '>(</span><span style='color:#00c4c4; '>'example hook ran'</span><span style='color:#d2cd86; '>)</span><span style='color:#b060b0; '>;</span>
  console<span style='color:#d2cd86; '>.</span><span style='color:#e66170; font-weight:bold; '>log</span><span style='color:#d2cd86; '>(</span>foo<span style='color:#d2cd86; '>,</span> <span style='color:#00c4c4; '>'foo'</span><span style='color:#d2cd86; '>)</span><span style='color:#b060b0; '>;</span>
  console<span style='color:#d2cd86; '>.</span><span style='color:#e66170; font-weight:bold; '>log</span><span style='color:#d2cd86; '>(</span>bar<span style='color:#d2cd86; '>,</span> <span style='color:#00c4c4; '>'bar'</span><span style='color:#d2cd86; '>)</span><span style='color:#b060b0; '>;</span>
<span style='color:#b060b0; '>}</span><span style='color:#d2cd86; '>)</span><span style='color:#b060b0; '>;</span>
hook<span style='color:#d2cd86; '>.</span>call<span style='color:#d2cd86; '>(</span><span style='color:#00c4c4; '>'example'</span><span style='color:#d2cd86; '>,</span> <span style='color:#00c4c4; '>'test'</span><span style='color:#d2cd86; '>,</span> <span style='color:#00c4c4; '>'test2'</span><span style='color:#d2cd86; '>)</span><span style='color:#b060b0; '>;</span>
</pre>