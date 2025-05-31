## Custom Wazuh Rule for Modbus Write Command Detection

```yaml
<group name="ics_modbus_write">
  <rule id="100010" level="10">
    <if_sid>65002</if_sid>
    <field name="data">Modbus Function Code 0x06</field>
    <description>Modbus Write Command Detected</description>
  </rule>
</group>
```

**Goal**: Alert if a Modbus "Write Single Register" command is seen on ICS network.

**Next Step**: Integrate with OpenPLC honeypot for testing.
