base/ — включает глобальные стили, такие как сброс стилей, типография, цвета и т.д.

components/ — содержит отдельные компоненты с отдельным файлом .scss для каждого из них.

layout/ — содержит стили для основных компонентов макета, таких как хедер, футер, навигация и т.д.

<!--
pages/ — содержит стили, специфичные для отдельных страниц, если это необходимо.

themes/ — стили для разных тем. -->

utils/ — глобальные миксины, функции, вспомогательные селекторы и т.д.

<!-- vendors/ — стили, миксины и прочее от третьих сторон -->

main.scss — выходной файл, в котором объединяются все стили.

.header {
padding-top: 24px;
padding-bottom: 25px;
}
.header .container {
display: flex;
align-items: baseline;
}
.navigation {
display: flex;
}
.logo {
margin-right: 93px;

font-family: "Raleway", sans-serif;
font-weight: 700;
font-size: 26px;
line-height: 1.192;
letter-spacing: 0.03em;
color: var(--hover-color);
}

.logo-second-part {
font-weight: 700;
font-size: 26px;
line-height: 1.192;
letter-spacing: 0.03em;
color: #000000;
}
.navigation-list {
display: flex;
align-items: center;
}

.navigation-list-link {
position: relative;
padding-bottom: 32px;
font-weight: 500;
font-size: 14px;
line-height: 1.143;
letter-spacing: 0.02em;
color: var(--secondary-font);

transition: color 250ms var(--transition-timing-function);
}
.current-page {
position: relative;
padding-bottom: 32px;
font-weight: 500;
font-size: 14px;
line-height: 1.143;
letter-spacing: 0.02em;
color: var(--hover-color);
}

.current-page::after {
content: "";
position: absolute;
left: 0;
bottom: 0;
width: 100%;
height: 4px;
background-color: var(--hover-color);
color: var(--hover-color);

transition: 250ms var(--transition-timing-function);
}

.navigation-list-item {
position: relative;
}

.navigation-list-item:not(:last-child) {
margin-right: 50px;
}

/_============END HEADER=========_/
