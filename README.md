BODY
----


<form id="form1" runat="server">
        <table style="width: 100%;">
            <tr>
                <td style="width: 2.5%"></td>
                <td style="width: 95%">&nbsp;</td>
                <td style="width: 2.5%"></td>
            </tr>
            <tr>
                <td style="width: 2.5%"></td>
                <td style="width: 95%">
                    <div class="container" style="background-color: white">
                        <div>
                            &nbsp;&nbsp;&nbsp;
                        </div>
                        <div>
                            <table class="StyleFormulario01" style="width: 100%;">
                                <tr>
                                    <td style="width: 2%"></td>
                                    <td style="width: 12.5%"></td>
                                    <td style="width: 2%"></td>
                                    <td style="width: 30.5%"></td>
                                    <td style="width: 6%"></td>
                                    <td style="width: 12.5%"></td>
                                    <td style="width: 2%"></td>
                                    <td style="width: 30.5%"></td>
                                    <td style="width: 2%"></td>
                                </tr>
                                <tr>
                                    <td style="width: 2%"></td>
                                    <td style="width: 12.5%"></td>
                                    <td style="width: 2%"></td>
                                    <td style="width: 30.5%"></td>
                                    <td style="width: 6%"></td>
                                    <td style="width: 12.5%"></td>
                                    <td style="width: 2%"></td>
                                    <td style="width: 30.5%"></td>
                                    <td style="width: 2%"></td>
                                </tr>
                            </table>
                        </div>
                        <div>
                            &nbsp;&nbsp;&nbsp;
                        </div>
                    </div>
                </td>
                <td style="width: 2.5%"></td>
            </tr>
            <tr>
                <td style="width: 2.5%"></td>
                <td style="width: 95%">&nbsp;</td>
                <td style="width: 2.5%"></td>
            </tr>
        </table>
    </form>













<table style="width: 100%;">
            <tr>
                <td style="width: 2.5%"></td>
                <td>


                </td>
                <td style="width: 2.5%"></td>
            </tr>
            <tr>
                <td style="width: 2.5%"></td>
                <td>
                    ----------------------------------------------------------------AQUI VA TITULO---------------------------------------------------------------- 

                    <div>
                         <h4>
                            <asp:Label ID="lblTITULO" runat="server" Text="TITULO"></asp:Label>
                        </h4>
                    </div>

                    <div>
                    </div>

                    <div style="position: relative; float: right;">
                    ----------------------------------------------------------------AQUI VAN BOTONES-------------------------------------------------------------- 

                        <asp:LinkButton ID="lbtnNuevo" runat="server" class="ibtn btn-primary" BorderStyle="Solid" ToolTip="GUARDAR" OnClick="lbtnNuevo_Click">
                            <asp:Image ID="Image1" runat="server" ImageUrl="~/img_app_1606/add_file-26.png" Width="20PX" Height="20px" />
                            <b>Nuevo</b>
                        </asp:LinkButton>

                        
                    </div>

                    <div>
                    </div>

                    <div>
                        <table class="StyleFormulario01">
                            <tr>
                                <td style="width: 2%"></td>
                                <td style="width: 12.5%"></td>
                                <td style="width: 2%"></td>
                                <td style="width: 30.5%"></td>
                                <td style="width: 6%"></td>
                                <td style="width: 12.5%"></td>
                                <td style="width: 2%"></td>
                                <td style="width: 30.5%"></td>
                                <td style="width: 2%"></td>
                            </tr>
                        </table>
                    </div>
                    
                </td>
                <td style="width: 2.5%"></td>
            </tr>
            <tr>
                <td style="width: 2.5%"></td>
                <td>&nbsp;
                </td>
                <td style="width: 2.5%"></td>
            </tr>
</table>

BOTON
-----

    <asp:LinkButton ID="lbtnNuevo" runat="server" class="ibtn btn-primary" BorderStyle="Solid" ToolTip="GUARDAR" OnClick="lbtnNuevo_Click">
        <asp:Image ID="Image1" runat="server" ImageUrl="~/img_app_1606/add_file-26.png" Width="20PX" Height="20px" />
        <b>Nuevo</b>
    </asp:LinkButton>

SUB-TITULO
----------

    <h3 class="page-header">
        Sub Titulo
    </h3>

TITULO
------

    <h4>
        <asp:Label ID="lblTITULO" runat="server" Text="TITULO"></asp:Label>
    </h4>


TEXTBOX
-------
 <asp:TextBox ID="txtTexto" runat="server" placeholder="TEXTO" CssClass ="form-control"></asp:TextBox></td>    

 BARRA
 -----
  <div id="dBarraSuperior">
                            
                            --POSISION IZQUIERDA--
                            <div style="position: relative; float: left;">
                                <input type="search" class="light-table-filter" data-table="order-table" placeholder="Buscar" style="width: 350px" tooltip="Ruc del cliente" />
                            </div>
                            

                            --POSISION DERECHA--   
                            <div style="position: relative; float: right;">
                                <asp:LinkButton ID="lbtnNuevo" runat="server" class="ibtn btn-primary" BorderStyle="Solid" ToolTip="GUARDAR" OnClick="lbtnNuevo_Click">
                                    <asp:Image ID="Image1" runat="server" ImageUrl="~/img_app_1606/add_file-26.png" Width="20PX" Height="20px" />
                                    <b>Nuevo</b>
                                </asp:LinkButton>

                                <asp:LinkButton ID="lbtnExport" runat="server" class="ibtn btn-primary" BorderStyle="Solid" ToolTip="GUARDAR">
                                    <asp:Image ID="Image2" runat="server" ImageUrl="~/img_app_1606/excel-26.png" Width="20PX" Height="20px" />
                                    <b>Exportar</b>
                                </asp:LinkButton>
                            </div>


                        </div>




CARGA DE DROPDOWLIST
--------------------

SBO_BEL.instancia.var1 = "ddlAutorizador";
ddlAutorizador.AppendDataBoundItems = true;
ddlAutorizador.DataSource = SSBO_BLL_APP1504.instancia.data_load_controls(SBO_BEL.instancia, pUsuarioActual).Tables[0];
ddlAutorizador.DataTextField = "usuario";
ddlAutorizador.DataValueField = "id";
ddlAutorizador.DataBind();



GRIDVIEW
--------
<asp:GridView ID="gvData" runat="server" OnSelectedIndexChanged="gvData_SelectedIndexChanged" class="table table-bordered" AllowSorting="True" OnSorting="gvData_Sorting" AutoGenerateColumns="False" >
                                        <Columns>
                                         <asp:CommandField HeaderText="" ShowSelectButton="True" SelectText="Ver" />
                                        <asp:BoundField DataField="nro_solicitud" HeaderText="N° SOL" SortExpression="nro_solicitud" HeaderStyle-HorizontalAlign="Center" HeaderStyle-VerticalAlign="Middle" />
                                        <asp:BoundField DataField="requerimiento" HeaderText="REQUERIMIENTO" SortExpression="requerimiento"/>
                                        <asp:BoundField DataField="usuario_responsable" HeaderText="USUARIO RESPONSABLE" SortExpression="usuario_responsable"/>
                                        <asp:BoundField DataField="area" HeaderText="AREA - CC" SortExpression="area"/>
                                        <asp:BoundField DataField="fecha_registro" HeaderText="FECHA DE REGISTRO" SortExpression="fecha_registro"/>
                                        <asp:BoundField DataField="fecha_validacion" HeaderText="FECHA DE VALIDACIÓN" SortExpression="fecha_validacion"/>
                                        <asp:BoundField DataField="fecha_aprobacion" HeaderText="FECHA DE APROBACIÓN" SortExpression="fecha_aprobacion"/>
                                        <asp:BoundField DataField="aprobador" HeaderText="APROBADOR" SortExpression="aprobador"/>
                                        <asp:BoundField DataField="fecha_entrega" HeaderText="FECHA DE ENTREGA" SortExpression="fecha_entrega"/>
                                        <asp:BoundField DataField="etapa" HeaderText="ESTADO" SortExpression="etapa"/>
                                        <asp:TemplateField>
                                            <HeaderTemplate>PROGRESO </HeaderTemplate>
                                            <ItemTemplate><asp:Image ID="Image2" runat="server" ImageUrl='<%# Eval("progreso") %>'  ToolTip='<%# Eval("tip") %>' /></ItemTemplate>
                                        </asp:TemplateField>
                                    </Columns>
                                </asp:GridView>




REPORTES
--------
A4 --> 4961;  7017



EJEMPLO HEAD BODY 6 FORMULARIOS CON TAB
---------------------------------------
<head runat="server">
    <title></title>
    <script src="http://10.31.2.20/ScaniaIT/Content_own/js/jquery_1120.min.js"></script>
    <script src="http://10.31.2.20/ScaniaIT/Content_own/js/jquery_2200.min.js"></script>
    <link href="http://10.31.2.20/ScaniaIT/Content_bootstrap336/css/bootstrap.min.css" rel="stylesheet" />
    <script src="http://10.31.2.20/ScaniaIT/Content_bootstrap336/js/jquery.min.js"></script>
    <script src="http://10.31.2.20/ScaniaIT/Content_bootstrap336/js/transition.js"></script>
    <script src="http://10.31.2.20/ScaniaIT/Content_bootstrap336/js/tab.js"></script>
    <script src="http://10.31.2.20/ScaniaIT/Content_bootstrap336/js/dropdown.js"></script>
    <script src="http://10.31.2.20/ScaniaIT/Content_bootstrap336/js/collapse.js"></script>
    <link href="http://10.31.2.20/ScaniaIT/Content_own/css/MySheet.css" rel="stylesheet" type="text/css" />

    <script>
        function loadStyleNavbar() {
            var vUrl = window.location.href;
            document.getElementById("Tab_t100").className = "active";
            document.getElementById("Ref_t100").className = "tab-pane fade active in";


            document.getElementById("Tab_t200").className = "...";
            document.getElementById("Ref_t200").className = "tab-pane fade";


            document.getElementById("Tab_t300").className = "...";
            document.getElementById("Ref_t300").className = "tab-pane fade";

            document.getElementById("Tab_t400").className = "...";
            document.getElementById("Ref_t400").className = "tab-pane fade";

            document.getElementById("Tab_t500").className = "...";
            document.getElementById("Ref_t500").className = "tab-pane fade";

            document.getElementById("Tab_t600").className = "...";
            document.getElementById("Ref_t600").className = "tab-pane fade";

            if (document.getElementById('<%= selectedTabs.ClientID %>').value == "Tab_t100") {
                document.getElementById("Tab_t100").className = "active";
                document.getElementById("Ref_t100").className = "tab-pane fade active in";
                document.getElementById("Tab_t200").className = "...";
                document.getElementById("Ref_t200").className = "tab-pane fade";
                document.getElementById("Tab_t300").className = "...";
                document.getElementById("Ref_t300").className = "tab-pane fade";
                document.getElementById("Tab_t400").className = "...";
                document.getElementById("Ref_t400").className = "tab-pane fade";
                document.getElementById("Tab_t500").className = "...";
                document.getElementById("Ref_t500").className = "tab-pane fade";
                document.getElementById("Tab_t600").className = "...";
                document.getElementById("Ref_t600").className = "tab-pane fade";
            }


            if (document.getElementById('<%= selectedTabs.ClientID %>').value == "Tab_t200") {

                document.getElementById("Tab_t100").className = "...";
                document.getElementById("Ref_t100").className = "tab-pane fade";
                document.getElementById("Tab_t200").className = "active";
                document.getElementById("Ref_t200").className = "tab-pane fade active in";
                document.getElementById("Tab_t300").className = "...";
                document.getElementById("Ref_t300").className = "tab-pane fade";
                document.getElementById("Tab_t400").className = "...";
                document.getElementById("Ref_t400").className = "tab-pane fade";
                document.getElementById("Tab_t500").className = "...";
                document.getElementById("Ref_t500").className = "tab-pane fade";
                document.getElementById("Tab_t600").className = "...";
                document.getElementById("Ref_t600").className = "tab-pane fade";
            }


            if (document.getElementById('<%= selectedTabs.ClientID %>').value == "Tab_t300") {
                document.getElementById("Tab_t100").className = "...";
                document.getElementById("Ref_t100").className = "tab-pane fade";
                document.getElementById("Tab_t200").className = "...";
                document.getElementById("Ref_t200").className = "tab-pane fade";
                document.getElementById("Tab_t300").className = "active";
                document.getElementById("Ref_t300").className = "tab-pane fade active in";
                document.getElementById("Tab_t400").className = "...";
                document.getElementById("Ref_t400").className = "tab-pane fade";
                document.getElementById("Tab_t500").className = "...";
                document.getElementById("Ref_t500").className = "tab-pane fade";
                document.getElementById("Tab_t600").className = "...";
                document.getElementById("Ref_t600").className = "tab-pane fade";
            }
            if (document.getElementById('<%= selectedTabs.ClientID %>').value == "Tab_t400") {
                document.getElementById("Tab_t100").className = "...";
                document.getElementById("Ref_t100").className = "tab-pane fade";
                document.getElementById("Tab_t200").className = "...";
                document.getElementById("Ref_t200").className = "tab-pane fade";
                document.getElementById("Tab_t300").className = "...";
                document.getElementById("Ref_t300").className = "tab-pane fade";
                document.getElementById("Tab_t400").className = "active";
                document.getElementById("Ref_t400").className = "tab-pane fade active in";
                document.getElementById("Tab_t500").className = "...";
                document.getElementById("Ref_t500").className = "tab-pane fade";
                document.getElementById("Tab_t600").className = "...";
                document.getElementById("Ref_t600").className = "tab-pane fade";
            }
            if (document.getElementById('<%= selectedTabs.ClientID %>').value == "Tab_t500") {
                document.getElementById("Tab_t100").className = "...";
                document.getElementById("Ref_t100").className = "tab-pane fade";
                document.getElementById("Tab_t200").className = "...";
                document.getElementById("Ref_t200").className = "tab-pane fade";
                document.getElementById("Tab_t300").className = "...";
                document.getElementById("Ref_t300").className = "tab-pane fade";
                document.getElementById("Tab_t400").className = "...";
                document.getElementById("Ref_t400").className = "tab-pane fade";
                document.getElementById("Tab_t500").className = "active";
                document.getElementById("Ref_t500").className = "tab-pane fade active in";
                document.getElementById("Tab_t600").className = "...";
                document.getElementById("Ref_t600").className = "tab-pane fade";
            }
            if (document.getElementById('<%= selectedTabs.ClientID %>').value == "Tab_t600") {
                document.getElementById("Tab_t100").className = "...";
                document.getElementById("Ref_t100").className = "tab-pane fade";
                document.getElementById("Tab_t200").className = "...";
                document.getElementById("Ref_t200").className = "tab-pane fade";
                document.getElementById("Tab_t300").className = "...";
                document.getElementById("Ref_t300").className = "tab-pane fade";
                document.getElementById("Tab_t400").className = "...";
                document.getElementById("Ref_t400").className = "tab-pane fade";
                document.getElementById("Tab_t500").className = "...";
                document.getElementById("Ref_t500").className = "tab-pane fade";
                document.getElementById("Tab_t600").className = "active";
                document.getElementById("Ref_t600").className = "tab-pane fade active in";
            }
        }
        document.addEventListener("DOMContentLoaded", loadStyleNavbar, false);


    </script>


</head>
<body>
    <form id="form1" runat="server">
        <input id="selectedTabs" type="hidden" value="" runat="server" />
        <table style="width: 100%;">
            <tr>
                <td style="width: 2.5%"></td>
                <td></td>
                <td style="width: 2.5%"></td>
            </tr>
            <tr>
                <td style="width: 2.5%"></td>
                <td>
                    <div class="container" style="background-color: white">
                        <div>
                            &nbsp;&nbsp;&nbsp;
                        </div>
                        <div>
                            <div style="position: relative; float: right;">

                                <asp:LinkButton ID="LinkButton1" runat="server" class="ibtn btn-primary" BorderStyle="Solid" ToolTip="ADJUNTAR DOCUMNETACIÓN">
                                    <asp:Image ID="Image2" runat="server" ImageUrl="~/img_app_1608/attach-26.png" Width="20PX" Height="20px" />
                                    <b>Adjuntar</b>
                                </asp:LinkButton>

                                <asp:LinkButton ID="lblSave" runat="server" class="ibtn btn-primary" BorderStyle="Solid" ToolTip="GUARDAR CAMBIOS EN EL REQUERIMIENTO">
                                    <asp:Image ID="Image3" runat="server" ImageUrl="~/img_app_1608/save-26.png" Width="20PX" Height="20px" />
                                    <b>Guardar</b>
                                </asp:LinkButton>
                            </div>
                            <h4>
                                <asp:Label ID="lblCliente" runat="server" Text="TITULO DE LA FUNCIONALIDAD"></asp:Label>
                            </h4>
                        </div>
                        <div>
                            &nbsp;&nbsp;&nbsp;
                        </div>
                        <ul id="myTab1" class="nav nav-tabs">
                            <li id="Tab_t100" onclick="document.getElementById('<%= selectedTabs.ClientID %>').value = 'Tab_t100'"><a href="#Ref_t100" data-toggle="tab">TITLE TAB01 EVENTO</a></li>
                            <li id="Tab_t200" onclick="document.getElementById('<%= selectedTabs.ClientID %>').value = 'Tab_t200'"><a href="#Ref_t200" data-toggle="tab">TITLE TAB02 EVENTO</a></li>
                            <li id="Tab_t300" onclick="document.getElementById('<%= selectedTabs.ClientID %>').value = 'Tab_t300'"><a href="#Ref_t300" data-toggle="tab">TITLE TAB03 EVENTO</a></li>
                            <li id="Tab_t400" onclick="document.getElementById('<%= selectedTabs.ClientID %>').value = 'Tab_t400'"><a href="#Ref_t400" data-toggle="tab">TITLE TAB04 EVENTO</a></li>
                            <li id="Tab_t500" onclick="document.getElementById('<%= selectedTabs.ClientID %>').value = 'Tab_t500'"><a href="#Ref_t500" data-toggle="tab">TITLE TAB05 EVENTO</a></li>
                            <li id="Tab_t600" onclick="document.getElementById('<%= selectedTabs.ClientID %>').value = 'Tab_t600'"><a href="#Ref_t600" data-toggle="tab">TITLE TAB06 EVENTO</a></li>
                        </ul>
                        <div>
                            &nbsp;&nbsp;&nbsp;
                        </div>
                        <div id="myTabContent1" class="tab-content">
                            <div class="tab-pane fade in active" id="Ref_t100">
                                <table class="StyleFormulario01">
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                </table>
                            </div>
                            <div class="tab-pane fade in active" id="Ref_t200">
                                <table class="StyleFormulario01">
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                </table>
                            </div>
                            <div class="tab-pane fade in active" id="Ref_t300">
                                <table class="StyleFormulario01">
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                </table>
                            </div>
                            <div class="tab-pane fade in active" id="Ref_t400">
                                <table class="StyleFormulario01">
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                </table>
                            </div>
                            <div class="tab-pane fade in active" id="Ref_t500">
                                <table class="StyleFormulario01">
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                </table>
                            </div>
                            <div class="tab-pane fade in active" id="Ref_t600">
                                <table class="StyleFormulario01">
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                    <tr>
                                        <td style="width: 2%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 6%"></td>
                                        <td style="width: 12.5%"></td>
                                        <td style="width: 2%"></td>
                                        <td style="width: 30.5%"></td>
                                        <td style="width: 2%"></td>
                                    </tr>
                                </table>
                            </div>
                        </div>
                    </div>
                </td>
                <td style="width: 2.5%"></td>
            </tr>
            <tr>
                <td style="width: 2.5%"></td>
                <td>&nbsp;
                </td>
                <td style="width: 2.5%"></td>
            </tr>
        </table>

    </form>
</body>


BUSCAR ARCHIVO DE TABLA
-----------------------


  <script type="text/javascript">
        (function (document) {
            'use strict';
            var LightTableFilter = (function (Arr) {
                var _input;
                function _onInputEvent(e) {
                    _input = e.target;
                    var tables = document.getElementsByClassName(_input.getAttribute('data-table'));
                    Arr.forEach.call(tables, function (table) {
                        Arr.forEach.call(table.tBodies, function (tbody) {
                            Arr.forEach.call(tbody.rows, _filter);
                        });
                    });
                }
                function _filter(row) {
                    var text = row.textContent.toLowerCase(), val = _input.value.toLowerCase();
                    row.style.display = text.indexOf(val) === -1 ? 'none' : 'table-row';
                }
                return {
                    init: function () {
                        var inputs = document.getElementsByClassName('light-table-filter');
                        Arr.forEach.call(inputs, function (input) {
                            input.oninput = _onInputEvent;

                            input.oninput = _onInputEvent;
                        });
                    }
                };
            })(Array.prototype);
            document.addEventListener('readystatechange', function () {
                if (document.readyState === 'complete') {
                    LightTableFilter.init();
                }
            });
        })(document);
    </script>
    
    
    
    
    <asp:GridView ID="gv_Data" runat="server" CssClass="pure-table order-table table" class="table table-bordered" AllowSorting="True" OnSorting="gv_Data_Sorting" Width="90%" OnRowDataBound="gv_Data_RowDataBound">
      <HeaderStyle BackColor="#EEC948" HorizontalAlign="Center" />
      <Columns>
        <asp:TemplateField>
          <ItemTemplate>
            <asp:ImageButton ID="ibtnSelect" runat="server" Height="20px" ImageUrl="~/img_app_1603/external_link-26.png" Width="20px" OnClick="ibtnSelect_Click" />
          </ItemTemplate>
        </asp:TemplateField>
      </Columns>
    </asp:GridView>
    
    
    
    
    
