# Realidade Aumentada Unity

### Aplicação Simples de Realidade Aumentada Unity + Vuforia

<p  align="justify"> A Unity e a Vuforia oferecem uma solução robusta para o desenvolvimento de aplicativos de Realidade Aumentada (AR), possibilitando que os desenvolvedores criem experiências impressionantes de AR para diversas aplicações..
</p>

<p  align="center">
<img src="https://gifs.eco.br/wp-content/uploads/2021/08/imagens-e-gifs-de-loading-4.gif">             
<br>


<p align="center">
<img src="imagens/vuforia-unity.png" width="460" height="300">
</p>

<!--GIF-->
<p align="center">
<img src="imagens/Gif_1.gif" width="460" height="300">
</p>

#### Para fazer uma aplicação como esta acima basta fazer o download do Vuforia Engine:

>  O Vuforia Engine pode ser facilmente importado para o Unity

[Download Vuforia](https://developer.vuforia.com/user/login?url=/downloads/sdk%3F_%3D1678117884)


>  É necessário criar uma conta e uma licença para registrar o seu Target (alvo).
> Após isso faça o Download do seus banco de dados (target+features).

<!--Target-->
<p align="center">
<img src="imagens/Target.png">
</p>


<!--Target-->
<p align="center">
<img src="imagens/targetmod.png">
</p>

> A Figura acima mostra o mapeamento para realidade aumentada.

#### Monte sua cena:

> Incluindo o Imagem Target e a Câmera AR

<!--Unity-1-->
<p align="center">
<img src="imagens/unity-1.png">
</p>

#### O script para rotacionar o Cubo

```javascript
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class rotate : MonoBehaviour
{
    public Vector3 rotateAmount;
    void Start()
    {
        
    }

    void Update()
    {
        transform.Rotate(rotateAmount * Time.deltaTime);
    }
}
```

#### Basta escolher o eixo de rotação e a módulo da posição nesse caso:
> X = 50, Y = 50, Z = 50.

<!--Detalhes-1-->
<p align="center">
<img src="imagens/Detalhes.png">
</p>

> O Unity é uma plataforma de desenvolvimento de jogos que também pode ser utilizada para desenvolver aplicativos de AR.

## Feliz 2023 

