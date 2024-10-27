<script setup>
import WelcomeItem from './WelcomeItem.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import ToolingIcon from './icons/IconTooling.vue'
import EcosystemIcon from './icons/IconEcosystem.vue'
import CommunityIcon from './icons/IconCommunity.vue'
import SupportIcon from './icons/IconSupport.vue'
</script>

<template>
  <WelcomeItem>
    <template #icon>
      <DocumentationIcon />
    </template>
    <template #heading>Analise de dados</template>

    <a href="">Ferramenta poderosa</a> que permite transformar grandes volumes de dados brutos em informações
    estratégicas e
    <a href="">insights acionáveis</a> para embasar decisões empresariais.
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <ToolingIcon />
    </template>
    <template #heading>Calculadora para caixas</template>

    <a href="">Otimizar o armazenamento e transporte</a>, calculando automaticamente o volume de produtos para garantir
    <a href="">o
      melhor
      aproveitamento de espaço nas caixas</a>. Este sistema utiliza as dimensões dos produtos (comprimento, largura e
    altura).

    <br />

  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <EcosystemIcon />
    </template>
    <template #heading>Integração com API para requerimentos</template>

    <a href="">Permite que sistemas interajam com um serviço externo</a> para gerenciar e manipular informações
    relacionadas a
    requerimentos. Este tipo de integração é crucial para automatizar processos.
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <CommunityIcon />
    </template>
    <template #heading>Chamada via e-mail</template>

    <a href="">Funcionalidade que permite a comunicação automatizada com usuários ou clientes</a> através do envio de
    mensagens eletrônicas. Esse recurso é frequentemente utilizado em sistemas de gerenciamento de requerimentos,
    notificações, marketing e suporte ao cliente.
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <SupportIcon />
    </template>
    <template #heading>Suporte com banco de dados</template>
    <a href="">Funcionalidade essencial em sistemas de informação que permite o armazenamento, gerenciamento e
      recuperação
      de dados de forma eficiente e segura.</a> Essa infraestrutura é fundamental para garantir a integridade,
    disponibilidade e acessibilidade das informações utilizadas em aplicações empresariais.
  </WelcomeItem>
</template>
