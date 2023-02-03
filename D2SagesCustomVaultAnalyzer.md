/* Sage's Vault Analyzer Super End-Game Edition | Highlights Trash | Keeps Top >.05% Armor */
(
(
	(
	is:weapon (is:sunset or is:blue)
	)
or
  (
	(is:armor -is:exotic -is:classitem)

	-(source:raid -is:dupelower -source:dcv)

	-(maxbasestatvalue:any)
	-(basestat:total:>=67)
    	-(basestat:highest:>=29)
    	-(basestat:highest&secondhighest:>=25.5)
    	-(basestat:highest&secondhighest&thirdhighest:>=19.666)
    	-(basestat:highest&secondhighest&thirdhighest&fourthhighest:>=15.75)
		-(basestat:highest&secondhighest&thirdhighest&fourthhighest&fifthhighest:>=13.2)
		-(basestat:highest&secondhighest&thirdhighest&fourthhighest&fifthhighest&sixthhighest:>=11.16)
  )
or
	(is:classitem energycapacity:<=9 -is:locked -(source:raid -is:dupelower -source:dcv))
or
	(is:armor is:sunset)
or
	(is:armor is:blue -(name:"war mantis" is:gauntlets))
or
	((is:armor or is:weapon) and (is:common or is:uncommon))
)
-(is:tagged -tag:junk -(tag:infuse -power:pinnaclecap)) -is:inloadout -is:masterwork -(is:armor -is:armor2.0) -(is:armor source:events) -name:classified
)  or (tag:junk -is:maxpowerloadout)
