2025-1-10 02:51:41
更新script.yaml文件，内容一键开关灯脚本
使用范例：
type: custom:button-card
entity: sensor.all_lights_num
layout: icon_name
show_icon: true
show_name: true
show_state: true
icon: mdi:lightbulb-group
name: 灯光
hold_action:
  action: call-service
  service: script.toggle_lights_unified
  service_data:
    lights:
      - light.can_ting_tong_deng_switch
      - light.shu_fang_deng_switch
      - light.can_ting_xi_ding_deng_switch
      - light.chu_fang_xi_ding_deng_switch
      - light.ke_ting_tong_deng_1_switch
      - light.ke_ting_tong_deng_2_switch
      - light.lang_deng_switch
      - light.ke_ting_deng_dai_switch
      - light.zhu_wo_deng_dai_switch
      - light.ke_wo_deng_switch
      - light.ci_wo_deng_switch
      - light.zhu_wei_ding_deng_switch
      - light.zhu_wei_jing_deng_switch
      - light.ke_wei_jing_deng_switch
      - light.ke_wei_ding_deng_switch
      - light.ke_ting_zhu_deng_switch
