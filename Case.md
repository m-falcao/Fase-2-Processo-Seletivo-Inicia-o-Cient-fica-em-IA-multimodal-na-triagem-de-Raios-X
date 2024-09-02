Como processo seletivo, vamos avaliar a capacidade dos candidatos de lidar com um problema muito próximo do que será encontrado durante a iniciação ciêntifica. Este projeto envolve não só lidar com a parte acadêmica de desenvolvimento de modelos, mas também com interagir com um ambiente de desenvolvimento e deploy real em ambiente hospitalar, como por exemplo interagir com PACs e arquivos DICOM.

Um PACS (Picture Archiving and Communication System) é um sistema de arquivamento e comunicação de imagens médicas que permite o armazenamento, acesso e compartilhamento digital de imagens radiológicas e outros tipos de exames em uma rede hospitalar.

Um arquivo DICOM (Digital Imaging and Communications in Medicine) é um formato padrão para armazenar e transmitir imagens médicas junto com informações associadas, permitindo a interoperabilidade entre diferentes sistemas de imagens médicas.

Neste contexto, para avaliação de habilidades técnicas, o candidato deverá entregar o seguinte desafio. As tarefas estão ordenadas em ordem de dificuldade. Pode fazer até onde conseguir.

1) Configurar e rodar um PACs OrthanC, utilizando Docker.
DICA: Já existem imagens pensadas para isso na internet. 

2) Utilizar um script Python para enviar arquivos DICOM (arquivos disponíveis nesse link).
DICA: Use API Rest do OrthanC.

3) Utilizando os mesmos arquivos DICOM, computar os resultados de classificação de achados utilizando o modelo pré-treinado e instruções encontradas na seção "Get Started"  do README do TorchXRayVision https://github.com/mlmed/torchxrayvision. 
DICA: Use a função da biblioteca xrv.utils.read_xray_dcm para ler arquivos DICOM.

4) EXTRA: Criar um DICOM SR (Structured Report) para cada arquivo DICOM com os resultados do modelo, e enviar os DICOM SR para o PACS local OrthanC. Note que o DICOM SR deve ser do paciente/estudo/série correta.

Os resultados devem ser entregues como um repositório no GitHub acessível publicamente. Além do código e Dockerfile, os resultados do TorchXRayVision devem estar no repositório em formato .json. Além disso, utilize o README do repositório para relatar de forma breve as dificuldades encontradas na solução deste desafio e o que você aprendeu neste processo.
