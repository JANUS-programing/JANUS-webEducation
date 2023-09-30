# HTML, CSS, JS

웹페이지는 우리가 일상에서 자주 마주치는 디지털 콘텐츠 중 하나입니다. 웹페이지의 구성과 디자인, 그리고 동작은 세 가지 핵심 기술, 즉 HTML, CSS, 그리고 JavaScript의 조합으로 이루어집니다. 각각은 웹페이지의 골격, 스타일, 그리고 기능을 담당하며, 함께 사용될 때 완전한 웹 경험을 제공합니다. 이 세 가지 기술은 웹 개발의 기초적이면서도 중심적인 역할을 하고 있습니다. 각각의 역할과 특성을 하나씩 알아보겠습니다.

- 마크업 언어
    
    마크업 언어는 태그 등을 이용하여 문서나 데이터의 구조를 명시하는 언어로, 해당 언어로 작성된 파일은 프로그램이 아닌 하나의 구조화된 문서로서의 성격을 가지게 됩니다.
    
    이러한 마크업 언어로 작성되는 파일로는 XML, HTML, 위키 등이 있습니다.
    
    그중 **HTML**은 웹페이지의 기본 구조를 기술하는 마크업 언어로, 페이지의 meta 정보와 전체적인 개형 및 형식을 정의합니다.
    
    웹 브라우저는 HTML이라는 언어가 갖는 태그를 이용하여 페이지 문서를 파싱하고, 해당 구조에 기반하여 사용자에게 페이지를 보여주게 됩니다.
    
- HTML
    
    위의 예시에서 말했듯이, HTML은 웹페이지의 기본 구조와 메타 정보에 대해 기술하는 언어입니다. `.html`확장자를 가지고 있으며, 브라우저가 읽을 수 있는 태그가 미리 정의되어 있어, 페이지를 작성 시 해당 태그를 이용하여 구조를 잡고, 각 태그의 내용에 해당 내용을 작성합니다.
    
    다음은 HTML로 작성된 “Hello, world!”라는 문장을 출력하는 웹페이지의 예시입니다.
    
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>HTML Intro</title>
    </head>
    <body>
        <h1>Hello, World!</h1>
    </body>
    </html>
    ```
    
    예시를 보고 감을 잡을 수 있듯, 부등호 `<>`를 이용하여 태그를 구별하며, 부등호 사이에는 태그의 종류, 각 태그 사이에는 해당 태그 의 형식을 상속할 내부 태그 혹은 내용이 담기게 됩니다. 해당 예시의 웹페이지 출력은 다음과 같습니다.
    
    // 결과 이미지 첨부
    
- CSS
    
    HTML만으로는 웹페이지의 구조를 정의하는 데는 충분하지만, 원하는 스타일과 디자인을 적용하기에는 한계가 있습니다. 때문에 흔히 마크업 언어 형태의 문서에 스타일을 주기 위해선 해당 문서의 스타일을 정의하는 시트가 필요하게 됩니다. CSS(Cascading Style Sheet)는 이러한 시트 역할을 할 수 있는 언어입니다. 즉 CSS는 웹페이지에서 페이지가 사용자에게 실제로 보여지는 스타일을 정의하는 역할을 합니다.
    
    CSS의 작성은 중괄호 앞에 스타일을 적용할 태그 및 id, class 등의 속성으로 구성된 “선택자”를 규정한 후, 해당 스타일에 대해 중괄호 안에 명시하는 방식으로 작성합니다.
    
    일례로 위의 “Helllo, Wolrd!”를 출력하는 페이지의 글자색을 붉은 색으로 바꾸고자 할때 css를 사용하면 다음과 같이 쓸 수 있습니다.
    
    ```html
    <!DOCTYPE html>
    <html lang="en">
    
    <head>
        <meta charset="UTF-8">
        <title>CSS Intro</title>
    		<!--
    			CSS문법을 이용하여 h1의 글자 색을 바꾸는 예제
    		-->
    		<style>
    			h1{
    				color : red;
    			}
    		</style>
    </head>
    
    <body>
        <h1>Hello, World!</h1>
    </body>
    </html>
    ```
    
    또는 아래와 같이 별도의 파일로 사용하는 것 또한 가능합니다.
    
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>CSS Intro</title>
    		<!--
    			CSS파일을 적용하여 스타일을 적용하는 예제
    		-->
    		<link href="style.css" rel="stylesheet">
    </head>
    <body>
    
        <h1>Hello, World!</h1>
    
    </body>
    </html>
    ```
    
    ```css
    /* style.css*/
    h1{
    	color : red;
    }
    ```
    

- Javascript
    
    웹페이지는 내용과 디자인이 아름답게 구성되어 있을지라도, 사용자와 상호작용하는 기능이 없다면 정적인 문서에 불과합니다. JavaScript (JS)는 웹페이지가 정적인 문서 이상의 기능을 하는 데에 중요한 역할을 합니다.
    
    JavaScript는 웹페이지의 조금 더 동적으로 보일 수 있게 합니다. 사용자가 버튼을 클릭하면 팝업이 나타나거나, 특정 영역에 마우스를 올리면 그래픽이 변경되는 등, 이런 동적인 행동들은 대부분 JavaScript로 구현됩니다. 그 뿐만 아니라, 웹페이지에서 서버로 데이터를 전송하거나 받아오는 과정 또한 JS를 통해 처리됩니다.
    
    JavaScript는 전통적인 프로그래밍 언어의 기능, 예를 들면 변수, 조건문, 함수 등을 모두 지원합니다. 처음에는 브라우저에서 직접 실행될 수 있는 인터프리터 언어로 시작했지만, 현재는 브라우저 외부에서도 활용되며, 그 범위가 꾸준히 확장되고 있습니다.
    
    다음은 JS를 이용하여 “Hello, Wolrd!”라는 문자열을 출력하는 페이지를 구현한 예제입니다.
    
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>HTML Intro</title>
    </head>
    <body>
        <script>
    			const body = document.queryselector("body");
    			const h1 = document.createElement("h1");
    			
    			h1.innerText = "Hello, World!";
    
    			body.appendChild(h1);
    		</script>
    </body>
    </html>
    ```
    
    마찬가지로 JS또한 파일 형태로 나누어 실행할 수 있습니다.
    
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>HTML Intro</title>
    </head>
    <body>
        <script src="app.js"></script>
    </body>
    
    </html>
    ```
    
    ```jsx
    const body = document.queryselector("body");
    const h1 = document.createElement("h1");
    			
    h1.innerText = "Hello, World!";
    
    body.appendChild(h1);
    ```