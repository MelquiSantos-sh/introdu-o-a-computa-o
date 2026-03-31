# introdu-o-a-computa-o
atividade de circuitos 
<?xml version="1.0" encoding="UTF-8" standalone="no"?>
<project source="2.7.1" version="1.0">
  This file is intended to be loaded by Logisim (http://www.cburch.com/logisim/).

  <lib desc="#Wiring" name="0"/>
  <lib desc="#Gates" name="1"/>
  <lib desc="#Plexers" name="2"/>
  <lib desc="#Arithmetic" name="3"/>
  <lib desc="#Memory" name="4"/>
  <lib desc="#I/O" name="5"/>
  <lib desc="#Base" name="6">
    <tool name="Text Tool">
      <a name="text" val=""/>
      <a name="font" val="SansSerif plain 12"/>
      <a name="halign" val="center"/>
      <a name="valign" val="base"/>
    </tool>
  </lib>
  <main name="half adder"/>
  <options>
    <a name="gateUndefined" val="ignore"/>
    <a name="simlimit" val="1000"/>
    <a name="simrand" val="0"/>
  </options>
  <mappings>
    <tool lib="6" map="Button2" name="Menu Tool"/>
    <tool lib="6" map="Button3" name="Menu Tool"/>
    <tool lib="6" map="Ctrl Button1" name="Menu Tool"/>
  </mappings>
  <toolbar>
    <tool lib="6" name="Poke Tool"/>
    <tool lib="6" name="Edit Tool"/>
    <tool lib="6" name="Text Tool">
      <a name="text" val=""/>
      <a name="font" val="SansSerif plain 12"/>
      <a name="halign" val="center"/>
      <a name="valign" val="base"/>
    </tool>
    <sep/>
    <tool lib="0" name="Pin">
      <a name="tristate" val="false"/>
    </tool>
    <tool lib="0" name="Pin">
      <a name="facing" val="west"/>
      <a name="output" val="true"/>
      <a name="labelloc" val="east"/>
    </tool>
    <tool lib="1" name="NOT Gate"/>
    <tool lib="1" name="AND Gate"/>
    <tool lib="1" name="OR Gate"/>
  </toolbar>
  <circuit name="half adder">
    <a name="circuit" val="half adder"/>
    <a name="clabel" val=""/>
    <a name="clabelup" val="east"/>
    <a name="clabelfont" val="SansSerif plain 12"/>
    <wire from="(300,110)" to="(300,210)"/>
    <wire from="(370,150)" to="(370,250)"/>
    <wire from="(540,130)" to="(640,130)"/>
    <wire from="(540,230)" to="(640,230)"/>
    <wire from="(300,110)" to="(490,110)"/>
    <wire from="(370,250)" to="(480,250)"/>
    <wire from="(300,210)" to="(480,210)"/>
    <wire from="(250,250)" to="(370,250)"/>
    <wire from="(250,210)" to="(300,210)"/>
    <wire from="(490,110)" to="(490,120)"/>
    <wire from="(370,150)" to="(490,150)"/>
    <comp lib="0" loc="(640,130)" name="Pin">
      <a name="facing" val="west"/>
      <a name="output" val="true"/>
      <a name="label" val="carry in"/>
      <a name="labelloc" val="east"/>
    </comp>
    <comp lib="1" loc="(540,230)" name="XOR Gate">
      <a name="inputs" val="2"/>
    </comp>
    <comp lib="0" loc="(250,210)" name="Pin">
      <a name="tristate" val="false"/>
      <a name="label" val="a"/>
    </comp>
    <comp lib="0" loc="(250,250)" name="Pin">
      <a name="tristate" val="false"/>
      <a name="label" val="b"/>
    </comp>
    <comp lib="0" loc="(640,230)" name="Pin">
      <a name="facing" val="west"/>
      <a name="output" val="true"/>
      <a name="label" val="s"/>
      <a name="labelloc" val="east"/>
    </comp>
    <comp lib="1" loc="(540,130)" name="AND Gate">
      <a name="inputs" val="2"/>
    </comp>
  </circuit>
  <circuit name="full adder">
    <a name="circuit" val="full adder"/>
    <a name="clabel" val=""/>
    <a name="clabelup" val="south"/>
    <a name="clabelfont" val="SansSerif plain 12"/>
    <wire from="(300,130)" to="(360,130)"/>
    <wire from="(300,290)" to="(360,290)"/>
    <wire from="(430,170)" to="(430,270)"/>
    <wire from="(470,210)" to="(470,310)"/>
    <wire from="(470,310)" to="(530,310)"/>
    <wire from="(300,130)" to="(300,290)"/>
    <wire from="(330,170)" to="(330,330)"/>
    <wire from="(330,170)" to="(360,170)"/>
    <wire from="(330,330)" to="(360,330)"/>
    <wire from="(420,310)" to="(470,310)"/>
    <wire from="(590,290)" to="(780,290)"/>
    <wire from="(430,170)" to="(550,170)"/>
    <wire from="(290,290)" to="(300,290)"/>
    <wire from="(600,190)" to="(670,190)"/>
    <wire from="(470,210)" to="(550,210)"/>
    <wire from="(410,150)" to="(670,150)"/>
    <wire from="(430,270)" to="(530,270)"/>
    <wire from="(290,330)" to="(330,330)"/>
    <wire from="(720,170)" to="(730,170)"/>
    <wire from="(730,20)" to="(730,170)"/>
    <wire from="(430,270)" to="(430,390)"/>
    <comp lib="0" loc="(780,290)" name="Pin">
      <a name="facing" val="west"/>
      <a name="output" val="true"/>
      <a name="label" val="S"/>
      <a name="labelloc" val="east"/>
    </comp>
    <comp lib="1" loc="(720,170)" name="OR Gate">
      <a name="inputs" val="2"/>
    </comp>
    <comp lib="1" loc="(600,190)" name="AND Gate">
      <a name="inputs" val="2"/>
    </comp>
    <comp lib="0" loc="(290,290)" name="Pin">
      <a name="tristate" val="false"/>
      <a name="label" val="A"/>
    </comp>
    <comp lib="0" loc="(430,390)" name="Pin">
      <a name="facing" val="north"/>
      <a name="tristate" val="false"/>
      <a name="label" val="carry in"/>
    </comp>
    <comp lib="0" loc="(730,20)" name="Pin">
      <a name="facing" val="south"/>
      <a name="output" val="true"/>
      <a name="label" val="carry out"/>
      <a name="labelloc" val="east"/>
    </comp>
    <comp lib="1" loc="(590,290)" name="XOR Gate">
      <a name="inputs" val="2"/>
    </comp>
    <comp lib="0" loc="(290,330)" name="Pin">
      <a name="tristate" val="false"/>
      <a name="label" val="B"/>
    </comp>
    <comp lib="1" loc="(420,310)" name="XOR Gate">
      <a name="inputs" val="2"/>
    </comp>
    <comp lib="1" loc="(410,150)" name="AND Gate">
      <a name="inputs" val="2"/>
    </comp>
  </circuit>
  <circuit name="somador mutiplos bits">
    <a name="circuit" val="somador mutiplos bits"/>
    <a name="clabel" val=""/>
    <a name="clabelup" val="east"/>
    <a name="clabelfont" val="SansSerif plain 12"/>
    <wire from="(500,180)" to="(750,180)"/>
    <wire from="(40,300)" to="(230,300)"/>
    <wire from="(590,140)" to="(590,150)"/>
    <wire from="(160,190)" to="(160,260)"/>
    <wire from="(40,260)" to="(160,260)"/>
    <wire from="(160,190)" to="(470,190)"/>
    <wire from="(240,270)" to="(240,280)"/>
    <wire from="(40,180)" to="(220,180)"/>
    <wire from="(480,200)" to="(480,210)"/>
    <wire from="(590,40)" to="(590,110)"/>
    <wire from="(370,260)" to="(370,270)"/>
    <wire from="(370,210)" to="(370,230)"/>
    <wire from="(260,290)" to="(750,290)"/>
    <wire from="(480,150)" to="(480,170)"/>
    <wire from="(40,160)" to="(340,160)"/>
    <wire from="(480,150)" to="(590,150)"/>
    <wire from="(340,160)" to="(340,240)"/>
    <wire from="(370,210)" to="(480,210)"/>
    <wire from="(200,250)" to="(200,280)"/>
    <wire from="(390,240)" to="(750,240)"/>
    <wire from="(430,180)" to="(470,180)"/>
    <wire from="(40,280)" to="(200,280)"/>
    <wire from="(200,250)" to="(360,250)"/>
    <wire from="(40,120)" to="(580,120)"/>
    <wire from="(340,240)" to="(360,240)"/>
    <wire from="(220,180)" to="(220,290)"/>
    <wire from="(430,140)" to="(430,180)"/>
    <wire from="(120,130)" to="(120,240)"/>
    <wire from="(40,240)" to="(120,240)"/>
    <wire from="(240,310)" to="(240,360)"/>
    <wire from="(220,290)" to="(230,290)"/>
    <wire from="(120,130)" to="(580,130)"/>
    <wire from="(40,140)" to="(430,140)"/>
    <wire from="(240,270)" to="(370,270)"/>
    <wire from="(610,120)" to="(750,120)"/>
    <comp lib="0" loc="(240,360)" name="Pin">
      <a name="facing" val="north"/>
      <a name="tristate" val="false"/>
      <a name="label" val="carry in "/>
    </comp>
    <comp lib="0" loc="(750,240)" name="Pin">
      <a name="facing" val="west"/>
      <a name="output" val="true"/>
      <a name="label" val="S1"/>
      <a name="labelloc" val="east"/>
    </comp>
    <comp loc="(390,240)" name="full adder">
      <a name="label" val="full adder 1"/>
      <a name="labelloc" val="south"/>
    </comp>
    <comp lib="0" loc="(40,120)" name="Pin">
      <a name="tristate" val="false"/>
      <a name="label" val="b3"/>
    </comp>
    <comp lib="0" loc="(750,290)" name="Pin">
      <a name="facing" val="west"/>
      <a name="output" val="true"/>
      <a name="label" val="S0"/>
      <a name="labelloc" val="east"/>
    </comp>
    <comp lib="0" loc="(750,180)" name="Pin">
      <a name="facing" val="west"/>
      <a name="output" val="true"/>
      <a name="label" val="S2"/>
      <a name="labelloc" val="east"/>
    </comp>
    <comp loc="(500,180)" name="full adder">
      <a name="label" val="full adder 2"/>
      <a name="labelloc" val="south"/>
    </comp>
    <comp lib="0" loc="(40,260)" name="Pin">
      <a name="tristate" val="false"/>
      <a name="label" val="a2"/>
    </comp>
    <comp lib="0" loc="(40,180)" name="Pin">
      <a name="tristate" val="false"/>
      <a name="label" val="b0"/>
    </comp>
    <comp lib="0" loc="(40,300)" name="Pin">
      <a name="tristate" val="false"/>
      <a name="label" val="a0"/>
    </comp>
    <comp loc="(610,120)" name="full adder">
      <a name="label" val="full adder 3"/>
      <a name="labelloc" val="south"/>
    </comp>
    <comp loc="(260,290)" name="full adder">
      <a name="label" val="full adder 0"/>
      <a name="labelloc" val="south"/>
    </comp>
    <comp lib="0" loc="(40,160)" name="Pin">
      <a name="tristate" val="false"/>
      <a name="label" val="b1"/>
    </comp>
    <comp lib="0" loc="(40,240)" name="Pin">
      <a name="tristate" val="false"/>
      <a name="label" val="a3"/>
    </comp>
    <comp lib="0" loc="(40,280)" name="Pin">
      <a name="tristate" val="false"/>
      <a name="label" val="a1"/>
    </comp>
    <comp lib="0" loc="(40,140)" name="Pin">
      <a name="tristate" val="false"/>
      <a name="label" val="b2"/>
    </comp>
    <comp lib="0" loc="(750,120)" name="Pin">
      <a name="facing" val="west"/>
      <a name="output" val="true"/>
      <a name="label" val="S3"/>
      <a name="labelloc" val="east"/>
    </comp>
    <comp lib="0" loc="(590,40)" name="Pin">
      <a name="facing" val="south"/>
      <a name="output" val="true"/>
      <a name="label" val="carry out"/>
      <a name="labelloc" val="east"/>
    </comp>
  </circuit>
  <circuit name="somador 8bits">
    <a name="circuit" val="somador 8bits"/>
    <a name="clabel" val=""/>
    <a name="clabelup" val="east"/>
    <a name="clabelfont" val="SansSerif plain 12"/>
    <comp lib="0" loc="(30,360)" name="Pin">
      <a name="tristate" val="false"/>
    </comp>
    <comp lib="0" loc="(30,150)" name="Pin">
      <a name="tristate" val="false"/>
    </comp>
    <comp lib="0" loc="(30,400)" name="Pin">
      <a name="tristate" val="false"/>
    </comp>
    <comp lib="0" loc="(30,340)" name="Pin">
      <a name="tristate" val="false"/>
    </comp>
    <comp lib="0" loc="(30,90)" name="Pin">
      <a name="tristate" val="false"/>
    </comp>
    <comp lib="0" loc="(30,110)" name="Pin">
      <a name="tristate" val="false"/>
    </comp>
    <comp lib="0" loc="(30,190)" name="Pin">
      <a name="tristate" val="false"/>
    </comp>
    <comp lib="0" loc="(30,280)" name="Pin">
      <a name="tristate" val="false"/>
    </comp>
    <comp lib="0" loc="(30,380)" name="Pin">
      <a name="tristate" val="false"/>
    </comp>
    <comp lib="0" loc="(30,320)" name="Pin">
      <a name="tristate" val="false"/>
    </comp>
    <comp lib="0" loc="(30,210)" name="Pin">
      <a name="tristate" val="false"/>
    </comp>
    <comp lib="0" loc="(30,300)" name="Pin">
      <a name="tristate" val="false"/>
    </comp>
    <comp lib="0" loc="(30,170)" name="Pin">
      <a name="tristate" val="false"/>
    </comp>
    <comp lib="0" loc="(30,130)" name="Pin">
      <a name="tristate" val="false"/>
    </comp>
    <comp lib="0" loc="(30,420)" name="Pin">
      <a name="tristate" val="false"/>
    </comp>
    <comp lib="0" loc="(30,230)" name="Pin">
      <a name="tristate" val="false"/>
    </comp>
  </circuit>
</project>
