# LifeCycle

## RUN
Angular CLI: 15.2.10
Node: 18.15.0

    npm install
    npm start

## NOTES

* @Input: colocado no componente filho para receber algo do componente pai
* @Output: colocado no componente filho para emitir algo para o componente pai

* ngOnInit: Este método é chamado depois que o Angular inicializou o componente. É útil para realizar inicializações, como buscar dados de um serviço ou configurar variáveis.

        ngOnInit(): void {
        // Lógica de inicialização aqui
        }

* ngOnChanges: Este método é chamado sempre que um valor de entrada (@Input) do componente é alterado. Ele fornece informações sobre as mudanças, como os valores antigos e novos.

        ngOnChanges(changes: SimpleChanges): void {
        // Lógica para lidar com mudanças nos inputs
        }

* ngOnDestroy: Este método é chamado quando o componente está prestes a ser destruído. É útil para realizar tarefas de limpeza, como cancelar assinaturas de Observables ou liberar recursos.

        ngOnDestroy(): void {
        // Lógica de limpeza aqui
        }

* ngAfterViewInit: Este método é chamado após a view do componente ter sido totalmente inicializada. É útil quando você precisa interagir com o DOM ou com os elementos da view.

        ngAfterViewInit(): void {
        // Lógica que depende da view aqui
        }

* ngDoCheck: Este método é chamado durante cada ciclo de detecção de mudanças. Pode ser útil para realizar verificações personalizadas ou lógica de atualização.

        ngDoCheck(): void {
        // Lógica de verificação personalizada aqui
        }


### Outros Hooks do Angular 

* AfterViewInit: Este hook é acionado após a visualização do componente ser totalmente inicializada. É útil para realizar ações específicas relacionadas à visualização, como manipulações no DOM ou integrações com bibliotecas externas.

* AfterViewChecked: Ativado após cada verificação da visualização do componente, permitindo a execução de ações adicionais nesse momento específico do ciclo de vida.

* AfterContentInit: Executado após a inicialização do conteúdo do componente. É útil quando operações dependem do conteúdo projetado no componente.

* AfterContentChecked: Ativado após cada verificação do conteúdo do componente, proporcionando oportunidades para ações adicionais relacionadas ao conteúdo.
