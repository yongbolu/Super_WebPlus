# META��ʶ
һ��ʲô��Viewport    
�ֻ�������ǰ�ҳ�����һ������ġ����ڡ���viewport���У�ͨ���������ġ����ڡ���viewport������Ļ�������Ͳ��ð�ÿ����ҳ������С�Ĵ����У��������ƻ�û������ֻ�������Ż�����ҳ�Ĳ��֣����û�����ͨ��ƽ�ƺ�����������ҳ�Ĳ�ͬ���֡��ƶ���� Safari ��������������� viewport ��� meta tag������ҳ������������ viewport �Ĵ�С�����ţ������ֻ������Ҳ����֧�֡�  

1. H5ҳ�洰���Զ��������豸��ȣ�����ֹ�û�����ҳ��    
`<meta name="viewport" content="width=device-width,initial-scale=1.0,minimum-scale=1.0,maximum-scale=1.0,user-scalable=no>`   
>˵����    
	width - viewport�Ŀ�� height - viewport�ĸ߶�  
	initial-scale - ��ʼ�����ű���  
	minimum-scale - �����û����ŵ�����С����  
	maximum-scale - �����û����ŵ���������  
	user-scalable - �û��Ƿ�����ֶ�����  

2. ���Խ�ҳ���е�����ʶ��Ϊ�绰����    
`<meta name="format-detection" content="telephone=no" />`
3. ����Androidƽ̨�ж������ַ��ʶ��    
`<meta name="format-detection" content="email=no" />`    

4. ����վ��ӵ�����Ļ����������ʽ�������ص�ַ���������ios��safari    
`<meta name="apple-mobile-web-app-capable" content="yes" />`    
`<!-- ios7.0�汾�Ժ�safari���ѿ�����Ч�� -->`
5. ����վ��ӵ�����Ļ����������ʽ�������ios��safari����״̬������ʽ      
`<meta name="apple-mobile-web-app-status-bar-style" content="black" />
<!-- ��ѡdefault��black��black-translucent -->`
6. viewportģ��    

    `<!DOCTYPE html>`    
    `<html>`    
    `<head>`    
    `<meta charset="utf-8">`    
    `<meta content="width=device-width,initial-scale=1.0,maximum-scale=1.0,user-scalable=no"    name="viewport">`    
    `<meta content="yes" name="apple-mobile-web-app-capable">`    
    `<meta content="black" name="apple-mobile-web-app-status-bar-style">`    
    `<meta content="telephone=no" name="format-detection">`    
    `<meta content="email=no" name="format-detection">`    
    `<title>����</title>`    
    `<link rel="stylesheet" href="index.css">`    
    `</head>`    
    `<body>`    
    `</body>`    
    `</html>`  

7. viewportģ�� �C target-densitydpi=device-dpi��android 2.3.5���°汾��֧��    

    `<!DOCTYPE html>`    
    `<html>`    
    `<head>`    
    `<meta charset="utf-8">`    
    `<meta name="viewport" content="width=750, user-scalable=no`    
    `target-densitydpi=device-dpi"><!-- widthȡֵ��ҳ�涨��Ŀ��һ�� -->`    
    `<meta content="yes" name="apple-mobile-web-app-capable">`    
    `<meta content="black" name="apple-mobile-web-app-status-bar-style">`    
    `<meta content="telephone=no" name="format-detection">`    
    `<meta content="email=no" name="format-detection">`    
    `<title>����</title>`    
    `<link rel="stylesheet" href="index.css">`    
    `</head>`    
    `<body>`    
    `</body>`    
    `</html>`
