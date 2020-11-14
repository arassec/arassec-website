---
home: true
heroImage: /profile.png
heroText: arassec.com
tagline: Andreas Sensen
features:
- title: 
  details: An open source project of mine to easily configure 'continuous workarounds'...
- title: 
  details: Thank you to JetBrains for providing me an open source license for their products!
footer: 
---

<script type="text/javascript">
document.createLogo = function(paragraph, targetLink, logo, logoSize, style) {
    let aTag = document.createElement('a');
    aTag.setAttribute('href', targetLink);
    let imgTag = document.createElement('img');
    imgTag.setAttribute('src', logo);
    imgTag.setAttribute('height', logoSize);
    imgTag.setAttribute('style', style);
    aTag.appendChild(imgTag);
    paragraph.prepend(document.createElement('br'));
    paragraph.prepend(document.createElement('br'));
    paragraph.prepend(aTag);
};

window.onload = function() {
    let paragraph = document.querySelector('.feature p');
    document.createLogo(paragraph, '/igor', 'igor-logo.png', '100');
    
    paragraph = document.querySelector('.feature:last-child p');
    document.createLogo(paragraph, 'https://www.jetbrains.com/?from=Igor', 'jetbrains.png', '100', 'margin-left: 90px;');
};

</script>