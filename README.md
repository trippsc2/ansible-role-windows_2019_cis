<!-- BEGIN_ANSIBLE_DOCS -->

# Ansible Role: trippsc2.windows_2019_cis
This role applies the CIS Benchmark hardening steps on Windows Server 2019 machines.

## Requirements

| Platform | Versions |
| -------- | -------- |
| Windows | 2019 |

## Dependencies

| Collection |
| ---------- |
| chocolatey.chocolatey |
| community.windows |

## Role Arguments
|Option|Description|Type|Required|Choices|Default|
|---|---|---|---|---|---|
| w2019cis_skip_reboot | Whether to skip rebooting the machine. | bool | no |  | false |
| w2019cis_level | The CIS Benchmark level to apply. Level 3 refers to Next Generation Windows Security (NGWS) benchmarks. | int | no | <ul><li>1</li><li>2</li><li>3</li></ul> | 1 |
| w2019cis_is_template | Whether to apply the CIS Benchmark as a template. If true, only apply the benchmarks that apply to standalone, domain members, and domain controllers are applied. | bool | no |  | false |
| w2019cis_rule_1_1_1_enabled | Whether to enable rule 1.1.1. | bool | no |  | true |
| w2019cis_rule_1_1_2_enabled | Whether to enable rule 1.1.2. | bool | no |  | true |
| w2019cis_rule_1_1_3_enabled | Whether to enable rule 1.1.3. | bool | no |  | true |
| w2019cis_rule_1_1_4_enabled | Whether to enable rule 1.1.4. | bool | no |  | true |
| w2019cis_rule_1_1_5_enabled | Whether to enable rule 1.1.5. | bool | no |  | true |
| w2019cis_rule_1_1_6_enabled | Whether to enable rule 1.1.6. | bool | no |  | true |
| w2019cis_password_history_size | The number of passwords to remember. | int | no |  | 24 |
| w2019cis_maximum_password_age | The maximum password age in days. | int | no |  | 365 |
| w2019cis_minimum_password_age | The minimum password age in days. | int | no |  | 1 |
| w2019cis_minimum_password_length | The minimum password length. | int | no |  | 14 |
| w2019cis_rule_1_2_1_enabled | Whether to enable rule 1.2.1. | bool | no |  | true |
| w2019cis_rule_1_2_2_enabled | Whether to enable rule 1.2.2. | bool | no |  | true |
| w2019cis_rule_1_2_3_enabled | Whether to enable rule 1.2.3. | bool | no |  | true |
| w2019cis_rule_1_2_4_enabled | Whether to enable rule 1.2.4. | bool | no |  | true |
| w2019cis_lockout_duration_in_minutes | The lockout duration in minutes. | int | no |  | 15 |
| w2019cis_lockout_bad_logon_count | The number of bad logon attempts before lockout. | int | no |  | 5 |
| w2019cis_lockout_reset_time_in_minutes | The lockout reset time in minutes. | int | no |  | 15 |
| w2019cis_rule_2_2_1_enabled | Whether to enable rule 2.2.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_2_enabled | Whether to enable rule 2.2.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_3_enabled | Whether to enable rule 2.2.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_4_enabled | Whether to enable rule 2.2.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_5_enabled | Whether to enable rule 2.2.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_6_enabled | Whether to enable rule 2.2.6. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_7_enabled | Whether to enable rule 2.2.7. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_8_enabled | Whether to enable rule 2.2.8. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_9_enabled | Whether to enable rule 2.2.9. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_10_enabled | Whether to enable rule 2.2.10. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_11_enabled | Whether to enable rule 2.2.11. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_12_enabled | Whether to enable rule 2.2.12. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_13_enabled | Whether to enable rule 2.2.13. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_14_enabled | Whether to enable rule 2.2.14. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_15_enabled | Whether to enable rule 2.2.15. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_16_enabled | Whether to enable rule 2.2.16. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_17_enabled | Whether to enable rule 2.2.17. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_18_enabled | Whether to enable rule 2.2.18. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_19_enabled | Whether to enable rule 2.2.19. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_20_enabled | Whether to enable rule 2.2.20. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_21_enabled | Whether to enable rule 2.2.21. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_22_enabled | Whether to enable rule 2.2.22. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_23_enabled | Whether to enable rule 2.2.23. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_24_enabled | Whether to enable rule 2.2.24. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_25_enabled | Whether to enable rule 2.2.25. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_26_enabled | Whether to enable rule 2.2.26. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_27_enabled | Whether to enable rule 2.2.27. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_28_enabled | Whether to enable rule 2.2.28. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_29_enabled | Whether to enable rule 2.2.29. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_30_enabled | Whether to enable rule 2.2.30. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_31_enabled | Whether to enable rule 2.2.31. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_32_enabled | Whether to enable rule 2.2.32. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_33_enabled | Whether to enable rule 2.2.33. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_34_enabled | Whether to enable rule 2.2.34. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_35_enabled | Whether to enable rule 2.2.35. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_36_enabled | Whether to enable rule 2.2.36. | bool | no |  | true |
| w2019cis_rule_2_2_37_enabled | Whether to enable rule 2.2.37. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_38_enabled | Whether to enable rule 2.2.38. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_39_enabled | Whether to enable rule 2.2.39. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_40_enabled | Whether to enable rule 2.2.40. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_41_enabled | Whether to enable rule 2.2.41. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_42_enabled | Whether to enable rule 2.2.42. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_43_enabled | Whether to enable rule 2.2.43. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_44_enabled | Whether to enable rule 2.2.44. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_45_enabled | Whether to enable rule 2.2.45. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_46_enabled | Whether to enable rule 2.2.46. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_47_enabled | Whether to enable rule 2.2.47. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_48_enabled | Whether to enable rule 2.2.48. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_2_36_force | Whether to override the level requirement for CIS rule 2.2.36. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_access_this_computer_from_the_network_additional_users | Additional users to grant `Access this computer from the network` permissions. | list of 'str' | no |  |  |
| w2019cis_adjust_memory_quotas_for_a_process_additional_users | Additional users to grant `Adjust memory quotas for a process` permissions. | list of 'str' | no |  |  |
| w2019cis_create_global_objects_additional_users | Additional users to grant `Create global objects` permissions. | list of 'str' | no |  |  |
| w2019cis_debug_programs_additional_users | Additional users to grant `Debug programs` permissions. | list of 'str' | no |  |  |
| w2019cis_generate_security_audits_additional_users | Additional users to grant `Generate security audits` permissions. | list of 'str' | no |  |  |
| w2019cis_impersonate_a_client_after_authentication_additional_users | Additional users to grant `Impersonate a client after authentication` permissions. | list of 'str' | no |  |  |
| w2019cis_manage_auditing_and_security_log_additional_users | Additional users to grant `Manage auditing and security log` permissions. | list of 'str' | no |  |  |
| w2019cis_perform_volume_maintenance_tasks_additional_users | Additional users to grant `Perform volume maintenance tasks` permissions. | list of 'str' | no |  |  |
| w2019cis_replace_a_process_level_token_additional_users | Additional users to grant `Replace a process level token` permissions. | list of 'str' | no |  |  |
| w2019cis_rule_2_3_1_1_enabled | Whether to enable rule 2.3.1.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_1_2_enabled | Whether to enable rule 2.3.1.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_1_3_enabled | Whether to enable rule 2.3.1.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_1_4_enabled | Whether to enable rule 2.3.1.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_1_5_enabled | Whether to enable rule 2.3.1.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_admin_username | The name to which to set the default Administrator account. | str | yes |  |  |
| w2019cis_guest_username | The name to which to set the default Guest account. | str | yes |  |  |
| w2019cis_rule_2_3_2_1_enabled | Whether to enable rule 2.3.2.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_2_2_enabled | Whether to enable rule 2.3.2.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_4_1_enabled | Whether to enable rule 2.3.4.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_4_2_enabled | Whether to enable rule 2.3.4.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_5_1_enabled | Whether to enable rule 2.3.5.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_5_2_enabled | Whether to enable rule 2.3.5.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_5_3_enabled | Whether to enable rule 2.3.5.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_5_4_enabled | Whether to enable rule 2.3.5.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_5_5_enabled | Whether to enable rule 2.3.5.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_6_1_enabled | Whether to enable rule 2.3.6.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_6_2_enabled | Whether to enable rule 2.3.6.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_6_3_enabled | Whether to enable rule 2.3.6.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_6_4_enabled | Whether to enable rule 2.3.6.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_6_5_enabled | Whether to enable rule 2.3.6.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_6_6_enabled | Whether to enable rule 2.3.6.6. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_maximum_machine_account_password_age_in_days | The maximum machine account password age in days. | int | no |  | 30 |
| w2019cis_rule_2_3_7_1_enabled | Whether to enable rule 2.3.7.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_7_2_enabled | Whether to enable rule 2.3.7.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_7_3_enabled | Whether to enable rule 2.3.7.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_7_4_enabled | Whether to enable rule 2.3.7.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_7_5_enabled | Whether to enable rule 2.3.7.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_7_6_enabled | Whether to enable rule 2.3.7.6. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_7_7_enabled | Whether to enable rule 2.3.7.7. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_7_8_enabled | Whether to enable rule 2.3.7.8. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_7_9_enabled | Whether to enable rule 2.3.7.9. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_7_6_force | Whether to override the level requirement for CIS rule 2.3.7.6. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_inactivity_timeout_in_seconds | The inactivity timeout in seconds. | int | no |  | 900 |
| w2019cis_legal_notice_text | The legal notice text. | str | no |  |  |
| w2019cis_legal_notice_caption | The legal notice caption. | str | no |  | DoD Notice and Consent Banner |
| w2019cis_cached_logons_count | The number of cached logons to remember. | int | no |  | 4 |
| w2019cis_password_expiry_warning_in_days | The password expiry warning in days. | int | no |  | 14 |
| w2019cis_smart_card_removal_behavior | The smart card removal behavior. | str | no | <ul><li>lock</li><li>logoff</li><li>disconnect</li></ul> | lock |
| w2019cis_rule_2_3_8_1_enabled | Whether to enable rule 2.3.8.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_8_2_enabled | Whether to enable rule 2.3.8.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_8_3_enabled | Whether to enable rule 2.3.8.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_9_1_enabled | Whether to enable rule 2.3.9.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_9_2_enabled | Whether to enable rule 2.3.9.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_9_3_enabled | Whether to enable rule 2.3.9.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_9_4_enabled | Whether to enable rule 2.3.9.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_9_5_enabled | Whether to enable rule 2.3.9.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019_idle_smb_timeout_in_minutes | The idle SMB timeout in minutes. | int | no |  | 15 |
| w2019cis_smb_spn_target_name_validation_level | The SMB SPN target name validation level. | str | no | <ul><li>accept</li><li>required</li></ul> | required |
| w2019cis_rule_2_3_10_1_enabled | Whether to enable rule 2.3.10.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_10_2_enabled | Whether to enable rule 2.3.10.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_10_3_enabled | Whether to enable rule 2.3.10.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_10_4_enabled | Whether to enable rule 2.3.10.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_10_5_enabled | Whether to enable rule 2.3.10.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_10_6_enabled | Whether to enable rule 2.3.10.6. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_10_7_enabled | Whether to enable rule 2.3.10.7. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_10_8_enabled | Whether to enable rule 2.3.10.8. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_10_9_enabled | Whether to enable rule 2.3.10.9. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_10_10_enabled | Whether to enable rule 2.3.10.10. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_10_11_enabled | Whether to enable rule 2.3.10.11. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_10_12_enabled | Whether to enable rule 2.3.10.12. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_10_13_enabled | Whether to enable rule 2.3.10.13. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_10_4_force | Whether to override the level requirement for CIS rule 2.3.10.4. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_null_session_pipes | The null session pipes. | list of 'str' | no |  |  |
| w2019cis_remote_registry_paths | The remote registry paths. | list of 'str' | no |  | ["System\\CurrentControlSet\\Control\\Print\\Printers", "System\\CurrentControlSet\\Services\\Eventlog", "Software\\Microsoft\\OLAP Server", "Software\\Microsoft\\Windows NT\\CurrentVersion\\Print", "Software\\Microsoft\\Windows NT\\CurrentVersion\\Windows", "System\\CurrentControlSet\\Control\\ContentIndex", "System\\CurrentControlSet\\Control\\Terminal Server", "System\\CurrentControlSet\\Control\\Terminal Server\\UserConfig", "System\\CurrentControlSet\\Control\\Terminal Server\\DefaultUserConfiguration", "Software\\Microsoft\\Windows NT\\CurrentVersion\\Perflib", "System\\CurrentControlSet\\Services\\SysmonLog"] |
| w2019cis_rule_2_3_11_1_enabled | Whether to enable rule 2.3.11.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_11_2_enabled | Whether to enable rule 2.3.11.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_11_3_enabled | Whether to enable rule 2.3.11.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_11_4_enabled | Whether to enable rule 2.3.11.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_11_5_enabled | Whether to enable rule 2.3.11.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_11_6_enabled | Whether to enable rule 2.3.11.6. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_11_7_enabled | Whether to enable rule 2.3.11.7. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_11_8_enabled | Whether to enable rule 2.3.11.8. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_11_9_enabled | Whether to enable rule 2.3.11.9. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_11_10_enabled | Whether to enable rule 2.3.11.10. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_ldap_client_signing_requirements | The LDAP client signing requirements. | str | no | <ul><li>require</li><li>negotiate</li></ul> | require |
| w2019cis_rule_2_3_13_1_enabled | Whether to enable rule 2.3.13.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_15_1_enabled | Whether to enable rule 2.3.15.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_15_2_enabled | Whether to enable rule 2.3.15.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_17_1_enabled | Whether to enable rule 2.3.17.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_17_2_enabled | Whether to enable rule 2.3.17.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_17_3_enabled | Whether to enable rule 2.3.17.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_17_4_enabled | Whether to enable rule 2.3.17.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_17_5_enabled | Whether to enable rule 2.3.17.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_17_6_enabled | Whether to enable rule 2.3.17.6. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_17_7_enabled | Whether to enable rule 2.3.17.7. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_2_3_17_8_enabled | Whether to enable rule 2.3.17.8. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_admin_uac_elevation_behavior | The UAC elevation behavior for administrators. | str | no | <ul><li>prompt_for_credentials</li><li>prompt_for_consent</li></ul> | prompt_for_consent |
| w2019cis_rule_5_1_enabled | Whether to enable rule 5.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_5_2_enabled | Whether to enable rule 5.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_5_2_force | Whether to override the level requirement for CIS rule 5.2. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_9_1_1_enabled | Whether to enable rule 9.1.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_9_1_2_enabled | Whether to enable rule 9.1.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_9_1_3_enabled | Whether to enable rule 9.1.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_9_1_4_enabled | Whether to enable rule 9.1.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_9_1_5_enabled | Whether to enable rule 9.1.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_9_1_6_enabled | Whether to enable rule 9.1.6. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_9_1_7_enabled | Whether to enable rule 9.1.7. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_9_1_8_enabled | Whether to enable rule 9.1.8. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_domain_firewall_log_path | The path to the domain firewall log. | str | no |  | %SystemRoot%\System32\logfiles\firewall\domainfw.log |
| w2019cis_domain_firewall_log_size_in_kb | The size of the domain firewall log in KB. | int | no |  | 16384 |
| w2019cis_rule_9_2_1_enabled | Whether to enable rule 9.2.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_9_2_2_enabled | Whether to enable rule 9.2.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_9_2_3_enabled | Whether to enable rule 9.2.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_9_2_4_enabled | Whether to enable rule 9.2.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_9_2_5_enabled | Whether to enable rule 9.2.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_9_2_6_enabled | Whether to enable rule 9.2.6. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_9_2_7_enabled | Whether to enable rule 9.2.7. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_9_2_8_enabled | Whether to enable rule 9.2.8. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_private_firewall_log_path | The path to the private firewall log. | str | no |  | %SystemRoot%\System32\logfiles\firewall\privatefw.log |
| w2019cis_private_firewall_log_size_in_kb | The size of the private firewall log in KB. | int | no |  | 16384 |
| w2019cis_rule_9_3_1_enabled | Whether to enable rule 9.3.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_9_3_2_enabled | Whether to enable rule 9.3.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_9_3_3_enabled | Whether to enable rule 9.3.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_9_3_4_enabled | Whether to enable rule 9.3.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_9_3_5_enabled | Whether to enable rule 9.3.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_9_3_6_enabled | Whether to enable rule 9.3.6. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_9_3_7_enabled | Whether to enable rule 9.3.7. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_9_3_8_enabled | Whether to enable rule 9.3.8. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_9_3_9_enabled | Whether to enable rule 9.3.9. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_9_3_10_enabled | Whether to enable rule 9.3.10. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_public_firewall_log_path | The path to the public firewall log. | str | no |  | %SystemRoot%\System32\logfiles\firewall\publicfw.log |
| w2019cis_public_firewall_log_size_in_kb | The size of the public firewall log in KB. | int | no |  | 16384 |
| w2019cis_rule_17_1_1_enabled | Whether to enable rule 17.1.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_17_1_2_enabled | Whether to enable rule 17.1.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_17_1_3_enabled | Whether to enable rule 17.1.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_17_2_1_enabled | Whether to enable rule 17.2.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_17_2_2_enabled | Whether to enable rule 17.2.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_17_2_3_enabled | Whether to enable rule 17.2.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_17_2_4_enabled | Whether to enable rule 17.2.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_17_2_5_enabled | Whether to enable rule 17.2.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_17_2_6_enabled | Whether to enable rule 17.2.6. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_17_3_1_enabled | Whether to enable rule 17.3.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_17_3_2_enabled | Whether to enable rule 17.3.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_17_4_1_enabled | Whether to enable rule 17.4.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_17_4_2_enabled | Whether to enable rule 17.4.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_17_5_1_enabled | Whether to enable rule 17.5.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_17_5_2_enabled | Whether to enable rule 17.5.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_17_5_3_enabled | Whether to enable rule 17.5.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_17_5_4_enabled | Whether to enable rule 17.5.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_17_5_5_enabled | Whether to enable rule 17.5.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_17_5_6_enabled | Whether to enable rule 17.5.6. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_17_6_1_enabled | Whether to enable rule 17.6.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_17_6_2_enabled | Whether to enable rule 17.6.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_17_6_3_enabled | Whether to enable rule 17.6.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_17_6_4_enabled | Whether to enable rule 17.6.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_17_7_1_enabled | Whether to enable rule 17.7.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_17_7_2_enabled | Whether to enable rule 17.7.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_17_7_3_enabled | Whether to enable rule 17.7.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_17_7_4_enabled | Whether to enable rule 17.7.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_17_7_5_enabled | Whether to enable rule 17.7.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_17_8_1_enabled | Whether to enable rule 17.8.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_17_9_1_enabled | Whether to enable rule 17.9.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_17_9_2_enabled | Whether to enable rule 17.9.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_17_9_3_enabled | Whether to enable rule 17.9.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_17_9_4_enabled | Whether to enable rule 17.9.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_17_9_5_enabled | Whether to enable rule 17.9.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_1_1_1_enabled | Whether to enable rule 18.1.1.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_1_1_2_enabled | Whether to enable rule 18.1.1.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_1_2_2_enabled | Whether to enable rule 18.1.2.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_1_3_enabled | Whether to enable rule 18.1.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_1_3_force | Whether to override the level requirement for CIS rule 18.1.3. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_3_1_enabled | Whether to enable rule 18.3.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_3_2_enabled | Whether to enable rule 18.3.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_3_3_enabled | Whether to enable rule 18.3.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_3_4_enabled | Whether to enable rule 18.3.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_3_5_enabled | Whether to enable rule 18.3.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_3_6_enabled | Whether to enable rule 18.3.6. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_laps_password_length | The LAPS password length. | int | no |  | 15 |
| w2019cis_laps_password_age_in_days | The LAPS password age in days. | int | no |  | 30 |
| w2019cis_rule_18_4_1_enabled | Whether to enable rule 18.4.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_4_2_enabled | Whether to enable rule 18.4.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_4_3_enabled | Whether to enable rule 18.4.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_4_4_enabled | Whether to enable rule 18.4.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_4_5_enabled | Whether to enable rule 18.4.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_4_6_enabled | Whether to enable rule 18.4.6. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_4_7_enabled | Whether to enable rule 18.4.7. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_5_1_enabled | Whether to enable rule 18.5.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_5_2_enabled | Whether to enable rule 18.5.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_5_3_enabled | Whether to enable rule 18.5.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_5_4_enabled | Whether to enable rule 18.5.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_5_5_enabled | Whether to enable rule 18.5.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_5_6_enabled | Whether to enable rule 18.5.6. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_5_7_enabled | Whether to enable rule 18.5.7. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_5_8_enabled | Whether to enable rule 18.5.8. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_5_9_enabled | Whether to enable rule 18.5.9. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_5_10_enabled | Whether to enable rule 18.5.10. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_5_11_enabled | Whether to enable rule 18.5.11. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_5_12_enabled | Whether to enable rule 18.5.12. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_5_5_force | Whether to override the level requirement for CIS rule 18.5.5. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_5_7_force | Whether to override the level requirement for CIS rule 18.5.7. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_5_10_force | Whether to override the level requirement for CIS rule 18.5.10. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_5_11_force | Whether to override the level requirement for CIS rule 18.5.11. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_screensaver_grace_period_in_seconds | The screensaver grace period in seconds. | int | no |  | 5 |
| w2019cis_rule_18_6_4_1_enabled | Whether to enable rule 18.6.4.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_6_4_2_enabled | Whether to enable rule 18.6.4.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_netbios_dns_resolution_behavior | The NetBIOS DNS resolution behavior. | str | no | <ul><li>disabled_on_public_networks</li><li>disabled</li></ul> | disabled_on_public_networks |
| w2019cis_rule_18_6_5_1_enabled | Whether to enable rule 18.6.5.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_6_5_1_force | Whether to override the level requirement for CIS rule 18.6.5.1. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_6_8_1_enabled | Whether to enable rule 18.6.8.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_6_9_1_enabled | Whether to enable rule 18.6.9.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_6_9_2_enabled | Whether to enable rule 18.6.9.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_6_9_1_force | Whether to override the level requirement for CIS rule 18.6.9.1. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_6_9_2_force | Whether to override the level requirement for CIS rule 18.6.9.2. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_6_10_2_enabled | Whether to enable rule 18.6.10.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_6_10_2_force | Whether to override the level requirement for CIS rule 18.6.10.2. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_6_11_2_enabled | Whether to enable rule 18.6.11.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_6_11_3_enabled | Whether to enable rule 18.6.11.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_6_11_4_enabled | Whether to enable rule 18.6.11.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_6_14_1_enabled | Whether to enable rule 18.6.14.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_6_19_2_1_enabled | Whether to enable rule 18.6.19.2.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_6_19_2_1_force | Whether to override the level requirement for CIS rule 18.6.19.2.1. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_6_20_1_enabled | Whether to enable rule 18.6.20.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_6_20_2_enabled | Whether to enable rule 18.6.20.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_6_20_1_force | Whether to override the level requirement for CIS rule 18.6.20.1. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_6_20_2_force | Whether to override the level requirement for CIS rule 18.6.20.2. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_6_21_1_enabled | Whether to enable rule 18.6.21.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_6_21_2_enabled | Whether to enable rule 18.6.21.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_6_21_2_force | Whether to override the level requirement for CIS rule 18.6.21.2. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_7_1_enabled | Whether to enable rule 18.7.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_7_2_enabled | Whether to enable rule 18.7.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_7_3_enabled | Whether to enable rule 18.7.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_7_4_enabled | Whether to enable rule 18.7.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_7_5_enabled | Whether to enable rule 18.7.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_7_6_enabled | Whether to enable rule 18.7.6. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_7_7_enabled | Whether to enable rule 18.7.7. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_7_8_enabled | Whether to enable rule 18.7.8. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_7_9_enabled | Whether to enable rule 18.7.9. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_7_10_enabled | Whether to enable rule 18.7.10. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_7_11_enabled | Whether to enable rule 18.7.11. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_7_1_force | Whether to override the level requirement for CIS rule 18.7.1. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rpc_listener_authentication_protocol | The RPC listener authentication protocol. | str | no | <ul><li>negotiate</li><li>kerberos</li></ul> | negotiate |
| w2019cis_rule_18_8_1_1_enabled | Whether to enable rule 18.8.1.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_8_1_1_force | Whether to override the level requirement for CIS rule 18.8.1.1. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_9_3_1_enabled | Whether to enable rule 18.9.3.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_4_1_enabled | Whether to enable rule 18.9.4.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_4_2_enabled | Whether to enable rule 18.9.4.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_5_1_enabled | Whether to enable rule 18.9.5.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_5_2_enabled | Whether to enable rule 18.9.5.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_5_3_enabled | Whether to enable rule 18.9.5.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_5_4_enabled | Whether to enable rule 18.9.5.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_5_5_enabled | Whether to enable rule 18.9.5.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_5_6_enabled | Whether to enable rule 18.9.5.6. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_5_7_enabled | Whether to enable rule 18.9.5.7. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_5_1_force | Whether to override the level requirement for CIS rule 18.9.5.1. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_9_5_2_force | Whether to override the level requirement for CIS rule 18.9.5.2. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_9_5_3_force | Whether to override the level requirement for CIS rule 18.9.5.3. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_9_5_4_force | Whether to override the level requirement for CIS rule 18.9.5.4. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_9_5_5_force | Whether to override the level requirement for CIS rule 18.9.5.5. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_9_5_6_force | Whether to override the level requirement for CIS rule 18.9.5.6. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_9_5_7_force | Whether to override the level requirement for CIS rule 18.9.5.7. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_vbs_platform_security_level | The VBS platform security level. | str | no | <ul><li>secure_boot</li><li>secure_boot_and_dma_protection</li></ul> | secure_boot |
| w2019cis_rule_18_9_7_2_enabled | Whether to enable rule 18.9.7.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_13_1_enabled | Whether to enable rule 18.9.13.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_19_2_enabled | Whether to enable rule 18.9.19.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_19_3_enabled | Whether to enable rule 18.9.19.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_19_4_enabled | Whether to enable rule 18.9.19.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_19_5_enabled | Whether to enable rule 18.9.19.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_20_1_1_enabled | Whether to enable rule 18.9.20.1.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_20_1_2_enabled | Whether to enable rule 18.9.20.1.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_20_1_3_enabled | Whether to enable rule 18.9.20.1.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_20_1_4_enabled | Whether to enable rule 18.9.20.1.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_20_1_5_enabled | Whether to enable rule 18.9.20.1.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_20_1_6_enabled | Whether to enable rule 18.9.20.1.6. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_20_1_7_enabled | Whether to enable rule 18.9.20.1.7. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_20_1_8_enabled | Whether to enable rule 18.9.20.1.8. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_20_1_9_enabled | Whether to enable rule 18.9.20.1.9. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_20_1_10_enabled | Whether to enable rule 18.9.20.1.10. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_20_1_11_enabled | Whether to enable rule 18.9.20.1.11. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_20_1_12_enabled | Whether to enable rule 18.9.20.1.12. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_20_1_13_enabled | Whether to enable rule 18.9.20.1.13. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_20_1_2_force | Whether to override the level requirement for CIS rule 18.9.20.1.2. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_9_20_1_3_force | Whether to override the level requirement for CIS rule 18.9.20.1.3. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_9_20_1_4_force | Whether to override the level requirement for CIS rule 18.9.20.1.4. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_9_20_1_6_force | Whether to override the level requirement for CIS rule 18.9.20.1.6. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_9_20_1_7_force | Whether to override the level requirement for CIS rule 18.9.20.1.7. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_9_20_1_8_force | Whether to override the level requirement for CIS rule 18.9.20.1.8. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_9_20_1_9_force | Whether to override the level requirement for CIS rule 18.9.20.1.9. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_9_20_1_10_force | Whether to override the level requirement for CIS rule 18.9.20.1.10. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_9_20_1_11_force | Whether to override the level requirement for CIS rule 18.9.20.1.11. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_9_20_1_12_force | Whether to override the level requirement for CIS rule 18.9.20.1.12. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_9_20_1_13_force | Whether to override the level requirement for CIS rule 18.9.20.1.13. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_9_23_1_enabled | Whether to enable rule 18.9.23.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_23_1_force | Whether to override the level requirement for CIS rule 18.9.23.1. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_9_24_1_enabled | Whether to enable rule 18.9.24.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_25_1_enabled | Whether to enable rule 18.9.25.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_25_1_force | Whether to override the level requirement for CIS rule 18.9.25.1. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_9_26_1_enabled | Whether to enable rule 18.9.26.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_26_1_force | Whether to override the level requirement for CIS rule 18.9.26.1. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_9_27_1_enabled | Whether to enable rule 18.9.27.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_27_2_enabled | Whether to enable rule 18.9.27.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_27_3_enabled | Whether to enable rule 18.9.27.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_27_4_enabled | Whether to enable rule 18.9.27.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_27_5_enabled | Whether to enable rule 18.9.27.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_27_6_enabled | Whether to enable rule 18.9.27.6. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_27_7_enabled | Whether to enable rule 18.9.27.7. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_30_1_enabled | Whether to enable rule 18.9.30.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_30_2_enabled | Whether to enable rule 18.9.30.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_30_1_force | Whether to override the level requirement for CIS rule 18.9.30.1. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_9_30_2_force | Whether to override the level requirement for CIS rule 18.9.30.2. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_9_32_6_1_enabled | Whether to enable rule 18.9.32.6.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_32_6_2_enabled | Whether to enable rule 18.9.32.6.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_32_6_3_enabled | Whether to enable rule 18.9.32.6.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_32_6_4_enabled | Whether to enable rule 18.9.32.6.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_32_6_1_force | Whether to override the level requirement for CIS rule 18.9.32.6.1. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_9_32_6_2_force | Whether to override the level requirement for CIS rule 18.9.32.6.2. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_9_34_1_enabled | Whether to enable rule 18.9.34.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_34_2_enabled | Whether to enable rule 18.9.34.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_35_1_enabled | Whether to enable rule 18.9.35.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_35_2_enabled | Whether to enable rule 18.9.35.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_35_2_force | Whether to override the level requirement for CIS rule 18.9.35.2. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_9_38_1_enabled | Whether to enable rule 18.9.38.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_whfb_roca_mitigation | The Windows Hello for Business ROCA mitigation. | str | no | <ul><li>block</li><li>audit</li></ul> | audit |
| w2019cis_rule_18_9_46_5_1_enabled | Whether to enable rule 18.9.46.5.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_46_11_1_enabled | Whether to enable rule 18.9.46.11.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_46_5_1_force | Whether to override the level requirement for CIS rule 18.9.46.5.1. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_9_46_11_1_force | Whether to override the level requirement for CIS rule 18.9.46.11.1. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_9_48_1_enabled | Whether to enable rule 18.9.48.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_48_1_force | Whether to override the level requirement for CIS rule 18.9.48.1. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_9_50_1_1_enabled | Whether to enable rule 18.9.50.1.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_50_1_2_enabled | Whether to enable rule 18.9.50.1.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_9_50_1_1_force | Whether to override the level requirement for CIS rule 18.9.50.1.1. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_9_50_1_2_force | Whether to override the level requirement for CIS rule 18.9.50.1.2. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_10_3_1_enabled | Whether to enable rule 18.10.3.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_3_1_force | Whether to override the level requirement for CIS rule 18.10.3.1. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_10_5_1_enabled | Whether to enable rule 18.10.5.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_7_1_enabled | Whether to enable rule 18.10.7.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_7_2_enabled | Whether to enable rule 18.10.7.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_7_3_enabled | Whether to enable rule 18.10.7.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_8_1_1_enabled | Whether to enable rule 18.10.8.1.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_10_1_enabled | Whether to enable rule 18.10.10.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_10_1_force | Whether to override the level requirement for CIS rule 18.10.10.1. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_10_12_1_enabled | Whether to enable rule 18.10.12.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_12_2_enabled | Whether to enable rule 18.10.12.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_13_1_enabled | Whether to enable rule 18.10.13.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_windows_connect_pin_requirement | The Windows Connect PIN requirement. | str | no | <ul><li>always</li><li>first_time</li></ul> | first_time |
| w2019cis_rule_18_10_14_1_enabled | Whether to enable rule 18.10.14.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_14_2_enabled | Whether to enable rule 18.10.14.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_15_1_enabled | Whether to enable rule 18.10.15.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_15_2_enabled | Whether to enable rule 18.10.15.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_15_3_enabled | Whether to enable rule 18.10.15.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_15_4_enabled | Whether to enable rule 18.10.15.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_15_5_enabled | Whether to enable rule 18.10.15.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_15_6_enabled | Whether to enable rule 18.10.15.6. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_15_7_enabled | Whether to enable rule 18.10.15.7. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_15_8_enabled | Whether to enable rule 18.10.15.8. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_15_2_force | Whether to override the level requirement for CIS rule 18.10.15.8. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_allow_telemetry | Whether to allow telemetry. | str | no | <ul><li>required</li><li>off</li></ul> | off |
| w2019cis_rule_18_10_17_1_enabled | Whether to enable rule 18.10.17.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_17_2_enabled | Whether to enable rule 18.10.17.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_17_3_enabled | Whether to enable rule 18.10.17.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_17_4_enabled | Whether to enable rule 18.10.17.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_26_1_1_enabled | Whether to enable rule 18.10.26.1.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_26_1_2_enabled | Whether to enable rule 18.10.26.1.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_26_2_1_enabled | Whether to enable rule 18.10.26.2.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_26_2_2_enabled | Whether to enable rule 18.10.26.2.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_26_3_1_enabled | Whether to enable rule 18.10.26.3.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_26_3_2_enabled | Whether to enable rule 18.10.26.3.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_26_4_1_enabled | Whether to enable rule 18.10.26.4.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_26_4_2_enabled | Whether to enable rule 18.10.26.4.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_application_log_max_size_in_kb | The maximum size of the Application log in KB. | int | no |  | 32768 |
| w2019cis_security_log_max_size_in_kb | The maximum size of the Security log in KB. | int | no |  | 196608 |
| w2019cis_setup_log_max_size_in_kb | The maximum size of the Setup log in KB. | int | no |  | 32768 |
| w2019cis_system_log_max_size_in_kb | The maximum size of the System log in KB. | int | no |  | 32768 |
| w2019cis_rule_18_10_29_2_enabled | Whether to enable rule 18.10.29.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_29_3_enabled | Whether to enable rule 18.10.29.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_29_4_enabled | Whether to enable rule 18.10.29.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_37_1_enabled | Whether to enable rule 18.10.37.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_37_1_force | Whether to override the level requirement for CIS rule 18.10.37.1. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_10_41_1_enabled | Whether to enable rule 18.10.41.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_41_1_force | Whether to override the level requirement for CIS rule 18.10.41.1. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_10_42_1_enabled | Whether to enable rule 18.10.42.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_43_5_1_enabled | Whether to enable rule 18.10.43.5.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_43_5_2_enabled | Whether to enable rule 18.10.43.5.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_43_6_1_1_enabled | Whether to enable rule 18.10.43.6.1.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_43_6_1_2_enabled | Whether to enable rule 18.10.43.6.1.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_43_6_3_1_enabled | Whether to enable rule 18.10.43.6.3.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_43_7_1_enabled | Whether to enable rule 18.10.43.7.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_43_10_1_enabled | Whether to enable rule 18.10.43.10.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_43_10_2_enabled | Whether to enable rule 18.10.43.10.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_43_10_3_enabled | Whether to enable rule 18.10.43.10.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_43_10_4_enabled | Whether to enable rule 18.10.43.10.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_43_12_1_enabled | Whether to enable rule 18.10.43.12.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_43_13_1_enabled | Whether to enable rule 18.10.43.13.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_43_13_2_enabled | Whether to enable rule 18.10.43.13.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_43_16_enabled | Whether to enable rule 18.10.43.16. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_43_17_enabled | Whether to enable rule 18.10.43.17. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_43_5_2_force | Whether to override the level requirement for CIS rule 18.10.43.5.2. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_10_43_7_1_force | Whether to override the level requirement for CIS rule 18.10.43.7.1. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_10_43_12_1_force | Whether to override the level requirement for CIS rule 18.10.43.12.1. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_10_51_1_enabled | Whether to enable rule 18.10.51.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_56_1_enabled | Whether to enable rule 18.10.56.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_56_1_force | Whether to override the level requirement for CIS rule 18.10.56.1. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_10_57_2_2_enabled | Whether to enable rule 18.10.57.2.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_57_3_2_1_enabled | Whether to enable rule 18.10.57.3.2.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_57_3_3_1_enabled | Whether to enable rule 18.10.57.3.3.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_57_3_3_2_enabled | Whether to enable rule 18.10.57.3.3.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_57_3_3_3_enabled | Whether to enable rule 18.10.57.3.3.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_57_3_3_4_enabled | Whether to enable rule 18.10.57.3.3.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_57_3_9_1_enabled | Whether to enable rule 18.10.57.3.9.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_57_3_9_2_enabled | Whether to enable rule 18.10.57.3.9.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_57_3_9_3_enabled | Whether to enable rule 18.10.57.3.9.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_57_3_9_4_enabled | Whether to enable rule 18.10.57.3.9.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_57_3_9_5_enabled | Whether to enable rule 18.10.57.3.9.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_57_3_10_1_enabled | Whether to enable rule 18.10.57.3.10.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_57_3_10_2_enabled | Whether to enable rule 18.10.57.3.10.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_57_3_11_1_enabled | Whether to enable rule 18.10.57.3.11.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_57_3_11_2_enabled | Whether to enable rule 18.10.57.3.11.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_57_3_2_1_force | Whether to override the level requirement for CIS rule 18.10.57.3.2.1. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_10_57_3_3_1_force | Whether to override the level requirement for CIS rule 18.10.57.3.3.1. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_10_57_3_3_3_force | Whether to override the level requirement for CIS rule 18.10.57.3.3.3. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_10_57_3_3_4_force | Whether to override the level requirement for CIS rule 18.10.57.3.3.4. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_10_57_3_10_1_force | Whether to override the level requirement for CIS rule 18.10.57.3.10.1. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_10_57_3_10_2_force | Whether to override the level requirement for CIS rule 18.10.57.3.10.2. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_10_58_1_enabled | Whether to enable rule 18.10.58.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_59_2_enabled | Whether to enable rule 18.10.59.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_59_3_enabled | Whether to enable rule 18.10.59.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_59_4_enabled | Whether to enable rule 18.10.59.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_59_2_force | Whether to override the level requirement for CIS rule 18.10.59.2. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_10_63_1_enabled | Whether to enable rule 18.10.63.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_63_1_force | Whether to override the level requirement for CIS rule 18.10.63.1. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_10_76_2_1_enabled | Whether to enable rule 18.10.76.2.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_80_1_enabled | Whether to enable rule 18.10.80.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_80_2_enabled | Whether to enable rule 18.10.80.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_80_1_force | Whether to override the level requirement for CIS rule 18.10.80.1. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_windows_ink_workspace_access | The Windows Ink Workspace access. | str | no | <ul><li>disallow_above_lock</li><li>disabled</li></ul> | disallow_above_lock |
| w2019cis_rule_18_10_81_1_enabled | Whether to enable rule 18.10.81.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_81_2_enabled | Whether to enable rule 18.10.81.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_81_3_enabled | Whether to enable rule 18.10.81.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_81_3_force | Whether to override the level requirement for CIS rule 18.10.81.3. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_10_82_1_enabled | Whether to enable rule 18.10.82.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_87_1_enabled | Whether to enable rule 18.10.87.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_87_2_enabled | Whether to enable rule 18.10.87.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_89_1_1_enabled | Whether to enable rule 18.10.89.1.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_89_1_2_enabled | Whether to enable rule 18.10.89.1.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_89_1_3_enabled | Whether to enable rule 18.10.89.1.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_89_2_1_enabled | Whether to enable rule 18.10.89.2.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_89_2_2_enabled | Whether to enable rule 18.10.89.2.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_89_2_3_enabled | Whether to enable rule 18.10.89.2.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_89_2_4_enabled | Whether to enable rule 18.10.89.2.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_89_2_5_enabled | Whether to enable rule 18.10.89.2.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_89_2_2_force | Whether to override the level requirement for CIS rule 18.10.89.2.2. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_10_90_1_enabled | Whether to enable rule 18.10.90.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_90_1_force | Whether to override the level requirement for CIS rule 18.10.90.1. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_18_10_92_2_1_enabled | Whether to enable rule 18.10.92.2.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_93_1_1_enabled | Whether to enable rule 18.10.93.1.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_93_2_1_enabled | Whether to enable rule 18.10.93.2.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_93_2_2_enabled | Whether to enable rule 18.10.93.2.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_93_4_1_enabled | Whether to enable rule 18.10.93.4.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_93_4_2_enabled | Whether to enable rule 18.10.93.4.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_18_10_93_4_3_enabled | Whether to enable rule 18.10.93.4.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_19_1_3_1_enabled | Whether to enable rule 19.1.3.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_19_1_3_2_enabled | Whether to enable rule 19.1.3.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_19_1_3_3_enabled | Whether to enable rule 19.1.3.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_screensaver_timeout_in_seconds | The screensaver timeout in seconds. | int | no |  | 900 |
| w2019cis_rule_19_5_1_1_enabled | Whether to enable rule 19.5.1.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_19_6_6_1_1_enabled | Whether to enable rule 19.6.6.1.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_19_6_6_1_1_force | Whether to override the level requirement for CIS rule 19.6.6.1.1. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_19_7_4_1_enabled | Whether to enable rule 19.7.4.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_19_7_4_2_enabled | Whether to enable rule 19.7.4.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_19_7_7_1_enabled | Whether to enable rule 19.7.7.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_19_7_7_2_enabled | Whether to enable rule 19.7.7.2. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_19_7_7_3_enabled | Whether to enable rule 19.7.7.3. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_19_7_7_4_enabled | Whether to enable rule 19.7.7.4. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_19_7_7_5_enabled | Whether to enable rule 19.7.7.5. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_19_7_7_3_force | Whether to override the level requirement for CIS rule 19.7.7.3. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_19_7_7_4_force | Whether to override the level requirement for CIS rule 19.7.7.4. This applies when the machine type is appropriate. | bool | no |  | false |
| w2019cis_rule_19_7_25_1_enabled | Whether to enable rule 19.7.25.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_19_7_40_1_enabled | Whether to enable rule 19.7.40.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_19_7_42_2_1_enabled | Whether to enable rule 19.7.42.2.1. This applies when the level and machine type are appropriate. | bool | no |  | true |
| w2019cis_rule_19_7_42_2_1_force | Whether to override the level requirement for CIS rule 19.7.42.2.1. This applies when the machine type is appropriate. | bool | no |  | false |


## License
MIT

## Author and Project Information
Jim Tarpley
<!-- END_ANSIBLE_DOCS -->
