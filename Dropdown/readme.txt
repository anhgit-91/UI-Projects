
1) overflow: hidden; 
++> show borders, but
--> ::before items can not be showed

*** We can use first child, last child to set border


2) Create a small triangle

dropdown__item:first-child:before {
	content: "";
	position: absolute;
	top: 0;
	left: 3rem;
	border-left: 10px solid transparent;
	border-right: 10px solid transparent;
	border-bottom: 10px solid var(--primary);
	transform: translateY(-100%);
}


3) Create a bridge to connect dropdown select and dropdown list


dropdown__list:before {
	content: "";
	height: 2.5rem;
	position: absolute;
	left: 0;
	right: 0;
	background-color: transparent;
	translate: transformY(-100%);
}
