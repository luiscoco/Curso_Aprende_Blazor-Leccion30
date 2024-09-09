# CURSO: Aprende Blazor

# LECCIÓN 30: Servicio NavigationManager (Parte 1)

1. Abrir la aplicación con Visual Studio 2022 o VSCode

2. Navegar a una ruta mediante código

```razor
@inject NavigationManager Navigation

<button @onclick="GoToPage">Go to About Page</button>

@code {
    void GoToPage()
    {
        // Navigating to the About page
        Navigation.NavigateTo("/about");
    }
}
```

3. Si queremos forzar el recargado de la página completa cuando navegamos a un componente  utilizamos este código:

```razor
Navigation.NavigateTo("/about", true);
```
