---
layout: page
title: SMUPal
description: Your SMUPal Assistant is here to you help with any question you have.
image: assets/images/chatbot.png
nav-menu: true
---

<html>

{% include head.html %}

<body>

{% include header.html %}

<section id="banner" class="style2">
    <div class="inner">
        <header class="major">
            <h1>{{ page.title }}</h1>
        </header>
        <div class="content">
            {{ page.description }}
            <p>Our virtual assistant is here to guide you through your journey at SMU. Whether you have questions about academics, student life, or university resources, our chatbot is ready to help!</p>
        </div>
    </div>
</section>

<section id="intro" class="wrapper style3">
    <div class="inner">
        <header class="major">
            <h2>How to Use the Chatbot</h2>
        </header>
        <p>Simply type your questions in the chat window, and our virtual assistant will respond with relevant information. Here are some example questions you can try:</p>
        <ul>
            <li><strong>What academic programs does SMU offer?</strong></li>
            <li><strong>How can I apply for financial aid?</strong></li>
            <li><strong>What resources are available for international students?</strong></li>
            <li><strong>Tell me about student clubs and events at SMU.</strong></li>
        </ul>
        <p>The chatbot is here to provide answers and connect you with the resources you need.</p>
    </div>
</section>

<section id="chatbot-container" class="wrapper style1">
    <div class="inner">
        <header class="major">
            <h2>Chat with Our Virtual Assistant</h2>
        </header>
        <p>Start interacting with our virtual assistant by clicking on the chat icon at the bottom right corner. The chatbot will load below.</p>
        <div id="chatbot-placeholder">
            <img src="{{ site.baseurl }}/assets/images/chatbot-placeholder.png" alt="Chatbot Placeholder" style="width:100%; max-width:500px; display:block; margin:auto;">
            <p style="text-align:center; margin-top:10px;">Chatbot will load here.</p>
        </div>
    </div>
</section>

{% include footer.html %}

<script>
  window.watsonAssistantChatOptions = {
    integrationID: "f1efb935-f751-4210-962c-7920ec52df19", // The ID of this integration.
    region: "aws-us-east-1", // The region your integration is hosted in.
    serviceInstanceID: "20241102-1216-2844-5062-615d243d7f1e", // The ID of your service instance.
    onLoad: async (instance) => { await instance.render(); }
  };
  
  setTimeout(function(){
    const t = document.createElement('script');
    t.src = "https://web-chat.global.assistant.watson.appdomain.cloud/versions/" + 
             (window.watsonAssistantChatOptions.clientVersion || 'latest') + 
             "/WatsonAssistantChatEntry.js";
    document.head.appendChild(t);
  }, 0);
</script>

</body>

</html>
