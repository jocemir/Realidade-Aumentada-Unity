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


#### Para fazer uma aplicação como esta  basta fazer o download do Vuforia 

>  O Vuforia Engine pode ser facilmente importado para o Unity

[Download Vuforia](https://developer.vuforia.com/user/login?url=/downloads/sdk%3F_%3D1678117884)


> Será necessário criar uma conta e uma licença para registrar o seu Target que será o alvo

> Em Seguida faça o Download do seu banco de dados (target+features)

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

#### Após escolha o eixo de rotação e o módulo da posição:>>

> X = 50, Y = 50, Z = 50.

<!--Detalhes-1-->
<p align="center">
<img src="imagens/Detalhes.png">
</p>

#### Agora vamos colocar movimento ao cubo inserindo o seguinte scritp:>>

```javascript
using System.Collections;

using System.Collections.Generic;

using UnityEngine;

public class Movimento : MonoBehaviour

{

    // Start is called before the first frame update

    Vector3 Vec;

    void Start()

    {

        

    }



    // Update is called once per frame

    void Update()

    {

        Vec = transform.localPosition;

        Vec.y += Input.GetAxis("Jump") * Time.deltaTime * 5;

        Vec.x += Input.GetAxis("Horizontal") * Time.deltaTime * 5;

        Vec.z += Input.GetAxis("Vertical") * Time.deltaTime * 5;

        transform.localPosition = Vec;

    }

}
```
### O Unity

<p  align="justify"> O Unity é uma plataforma de desenvolvimento de jogos e experiências interativas em 2D e 3D. Ele fornece uma variedade de ferramentas e recursos para criar jogos e experiências interativas, incluindo gráficos em tempo real, física simulada, áudio, animação, scripting e suporte para vários dispositivos e plataformas.
</p>




## Feliz 2023 :)

