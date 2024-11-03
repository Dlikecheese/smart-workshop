<template>
  <div>
    <header class="w-full bg-blue-800">
      <div
        style="background-color: rgb(2 70 190 / 7%)"
        class="flex justify-between items-center px-[60px] h-[90px] pr-[200px] pt-2"
      >
        <img src="@/assets/logo.png" alt="" width="280px" />
        <div class="flex items-center mr-4 text-white relative -top-1">
          <span class="mr-2">欢迎您</span>
          <img
            src="@/assets/person/huangxiujuan.png"
            alt=""
            class="cursor-pointer w-[40px] h-[40px] rounded-full ml-2"
          />
        </div>
      </div>
    </header>
  </div>

  <div class="box px-40 py-6">
    <div class="content p-10">
      <div v-if="type === 'person'">
        <p class="text-center text-2xl mb-4">企业工程师介绍</p>
        <div class="flex justify-center items-center flex-col gap-4 mb-6">
          <img src="@/assets/teacher-desc.png" alt="" />
          <span class="text-xl">刘天宋，首创高科技术服务有限公司技术总监</span>
        </div>
        <div class="desc leading-6">
          <div class="indent-8 mb-2">
            作为企业物联网领域的杰出项目工程师，他以其深厚的技术功底和丰富的项目经验，在行业内享有高度评价。投身于物联网技术的研发与应用，专注于将前沿科技转化为实际生产力，为众多企业带来了显著的效益提升。
          </div>
          <div class="indent-8 mb-2">
            他精通物联网架构的设计与优化，还深入掌握了多种关键技术，包括各类传感器应用、RFID技术、以及Wi-Fi、LoRa、NB-IoT等无线通信协议。此外，他在云计算平台（如阿里云IoT、华为云IoT等）的集成与应用方面也有着丰富的实践经验，能够高效地实现物联网设备与云端的无缝对接，为项目提供强大的数据处理与分析能力。
          </div>
          <div class="indent-8 mb-2">
            在中国中车数字工厂管理平台的项目中，他作为技术负责人，成功设计并实施了一套全面的物联网解决方案。该方案通过集成各类生产设备与传感器，实现了生产过程的实时监控与智能调度，显著提高了生产效率与产品质量。此外，在我市智慧城市项目中，他带领团队克服了重重技术难题，成功构建了覆盖城市关键区域的物联网监测网络，为城市管理与服务提供了有力的数据支持。
          </div>
          <div class="indent-8 mb-2">
            作为企业物联网项目工程师，凭借其深厚的技术功底、丰富的项目经验以及出色的管理与协作能力，在物联网领域取得了显著的成就。他将继续致力于将前沿科技应用于实际项目中，为企业创造更大的价值。
          </div>
        </div>
      </div>

      <div v-if="type === 'company'">
        <p class="text-center text-2xl mb-4">数字车间集控平台搭建</p>
        <div class="leading-6">
          <p class="mb-4">一、项目背景</p>
          <div class="indent-8 mb-4 leading-8">
            随着智能制造和工业4.0时代的到来，传统制造业正面临着前所未有的转型压力。为了提高生产效率、降低成本、增强市场竞争力，实现生产过程的数字化、网络化和智能化已成为行业共识。数字车间作为智能制造的重要组成部分，通过集成信息技术、自动化技术和智能管理技术，能够显著提升生产线的灵活性和响应速度，确保产品质量，优化资源配置。因此，搭建一个高效、可靠的数字车间集控平台，对于推动制造业转型升级具有重要意义。
          </div>

          <div class="flex items-center justify-center mb-8">
            <img
              src="@/assets/company/chejianDetail.png"
              alt=""
              width="800px"
            />
          </div>

          <p class="mb-4">二、项目目标</p>
          <div class="mb-4">
            <div class="mb-2 indent-8">
              本项目旨在构建一套全面、集成的数字车间集控平台，实现以下核心目标：
              生产数据集成：整合车间内各类生产设备、传感器、监控系统等产生的数据，形成统一的数据湖，为后续分析与决策提供基础。
            </div>
            <div class="mb-2 indent-8">
              实时监控与预警：通过实时监控生产状态、设备健康状况及工艺参数，及时发现异常并触发预警机制，减少停机时间和质量损失。
            </div>
            <div class="mb-2 indent-8">
              智能调度与优化：运用先进算法对生产任务进行智能排程，优化资源配置，提高生产效率和灵活性。
            </div>
            <div class="mb-2 indent-8">
              质量追溯与管理：建立产品全生命周期的质量追溯体系，确保产品质量可追溯，便于问题定位与改进。
            </div>
            <div class="mb-2 indent-8">
              远程运维与诊断：支持设备的远程监控、故障诊断与维护，降低维护成本，提升设备利用率。
            </div>
            <div class="mb-2 indent-8">
              决策支持与分析：基于大数据分析，为管理层提供生产绩效、成本分析、市场趋势预测等决策支持信息。
            </div>
          </div>

          <p class="mb-4">三、项目内容</p>
          <div class="mb-4">
            <div class="mb-2 indent-8">
              硬件集成与升级：评估现有设备状况，进行必要的硬件升级或新增智能设备，如传感器、工业机器人、智能仪表等，确保数据采集的准确性和实时性。
            </div>
            <div class="mb-2 indent-8">
              软件平台开发：设计并开发集控平台软件，包括数据采集层、数据处理层、应用服务层等，实现数据的整合、处理、展示与分析功能。
            </div>
            <div class="mb-2 indent-8">
              网络架构搭建：构建安全、稳定的车间内部网络，确保数据的高效传输与安全，同时考虑与外部系统的对接能力。
            </div>
            <div class="mb-2 indent-8">
              系统测试与优化：进行系统集成测试，验证平台功能与性能，根据测试结果进行调优，确保平台稳定运行。
            </div>
            <div class="mb-2 indent-8">
              培训与实施：对车间操作人员、管理人员进行系统操作培训，制定详细的实施计划，逐步推进平台在车间内的应用。
            </div>
          </div>

          <p class="mb-4">四、预期成果</p>
          <div class="mb-4">
            <div class="mb-2 indent-8">
              生产效率提升：通过智能化管理，预计生产效率可提高20%以上。
            </div>
            <div class="mb-2 indent-8">
              成本降低：减少因故障停机、物料浪费等造成的成本，预计成本节约可达15%。
            </div>
            <div class="mb-2 indent-8">
              质量控制增强：建立严格的质量控制体系，产品不良率显著降低。
            </div>
            <div class="mb-2 indent-8">
              决策效率提高：为管理层提供及时、准确的数据支持，加快决策过程。
            </div>
            <div class="mb-2 indent-8">
              创新能力提升：构建开放、可扩展的平台架构，为未来的技术创新和升级奠定坚实基础。
            </div>
          </div>
        </div>
      </div>

      <div v-if="type === 'course'">
        <p class="text-center text-2xl mb-4">数字车间</p>
        <div class="leading-6">
          数字车间课程通常涵盖了智能制造、自动化技术、信息技术、机械制造和物流管理等多个技术领域。这些课程旨在帮助学习者理解数字化车间的基本概念、关键技术和应用实践，以及如何通过数字化转型提升制造企业的竞争力。以下是一些具体的数字车间课程介绍：<br />
          1. GB/T 37393-2019《数字化车间 通用技术要求》和GB/T
          37413-2019《数字化车间 术语和定义》国家标准解读：<br />
          o
          该课程详细介绍了数字化车间建设在智能制造中的重要作用，当前存在的主要问题，以及数字化车间的关键要素。课程还详细解读了《数字化车间通用技术要求》各章节的主要内容，并通过示范案例展示了数字化车间建设的效果，以及基于该标准进行诊断评估的方法体系。
          2. 工业互联网+智能工厂与数字化无人车间建设专题培训班： o
          该培训班涵盖了工业互联网的发展、智能制造中的数字化转型、智慧工厂的顶层设计、ET工业大脑赋能制造业、无人工厂和无人车间的变革与未来等多个模块。课程旨在帮助学员全面了解智能工厂和数字化车间的构建方法和实践案例。<br />
          3. 智能生产线数字化设计与仿真： o
          该课程主要学习机电一体化概念设计解决方案（MCD），适用于机电一体化产品的概念设计。课程内容包括NX
          MCD软件的各种功能和操作方法，以及如何进行3D建模和仿真。通过实际操作案例，学习者能够更好地理解和掌握NX
          MCD软件。<br />
          4. 《数字化工厂技术与应用》课程教学大纲： o
          该课程旨在使学生理解数字化工厂相关制造领域的基本知识，掌握数字化工厂的运作及管理过程，以及产品开发数字化、生产准备数字化、制造数字化、管理数字化等智能制造方法。课程强调了数字化制造技术的重要性，并探讨了数字化工厂技术的应用和实践。<br />
          5. 数字化虚拟仿真基础（视频课）： o
          该课程向学员介绍了工厂仿真及其基本应用，包括工业工厂仿真的概念、工具和意义，以及人机作业仿真、物流仿真和生产仿真等内容。课程旨在使学员掌握数字化转型的核心概念和工具，并能够使用仿真工具来实现工厂自动化和优化。<br />
          6. 《数字化与智能化车间》： o
          本书介绍了数字化智能化车间的基本概念，提出了数字化智能化车间的体系架构模型，并对数字化智能化车间技术体系中的虚拟车间建模与仿真优化、制造物联网技术及应用、生产过程智能管控等关键内容进行了深入探讨。书中还结合了企业应用案例进行详细说明。
          这些课程和资源为学习者提供了全面的数字车间知识和技能，帮助他们在数字化转型的浪潮中保持竞争力。
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.box {
  background-color: #f5f5f5;
}

.content {
  background-color: #fff;
  min-height: calc(100vh - 120px);
}

p {
  font-weight: 600;
}
</style>
<script setup lang="ts">
import { ref } from 'vue'
import { useRouter } from 'vue-router'
import { UserOutlined } from '@ant-design/icons-vue'

const router = useRouter()
const type = ref(router.currentRoute.value.query.type)
</script>
