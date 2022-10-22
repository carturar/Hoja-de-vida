# Proyecto Hoja de Vida

Proyecto en grupo hojas de vida usando html5, css3, boostrap, javascript

## Instalación

se interlaza html con css, haciendo un llamado de las librerias de boostrap y javascript para enriqueser mas la hja de vida


## Usando

``` JavaScript
window.addEventListener('DOMContentLoaded', event => {

    // Activate Bootstrap scrollspy on the main nav element
    const sideNav = document.body.querySelector('#sideNav');
    if (sideNav) {
        new bootstrap.ScrollSpy(document.body, {
            target: '#sideNav',
            offset: 74,
        });
    };

    // Collapse responsive navbar when toggler is visible
    const navbarToggler = document.body.querySelector('.navbar-toggler');
    const responsiveNavItems = [].slice.call(
        document.querySelectorAll('#navbarResponsive .nav-link')
    );
    responsiveNavItems.map(function (responsiveNavItem) {
        responsiveNavItem.addEventListener('click', () => {
            if (window.getComputedStyle(navbarToggler).display !== 'none') {
                navbarToggler.click();
            }
        });
    });

});

```

## Realizada por 


####Carlos Arturo Arias Ospina
####Viviana Restrepo Quintero
####Luis Javier Velez uribe

## License
[MIT](https://choosealicense.com/licenses/mit/)
Creative Commons Attribution 3.0 Unported
http://creativecommons.org/licenses/by/3.0/
