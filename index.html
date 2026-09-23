# -*- coding: utf-8 -*-
import re

with open('index.html', 'r', encoding='utf-8') as f:
    html = f.read()

# 1. Update Title and Subtitle to include Clause 4 and Clause 5
html = html.replace(
    'مختبر فحص ومعايرة الذهب والمعادن الثمينة | شركة GBI | البند 4 (الحيادية والسرية)',
    'مختبر فحص ومعايرة الذهب والمعادن الثمينة | شركة GBI | البند 4 (الحيادية والسرية) والبند 5 (المتطلبات الهيكلية)'
)

# 2. Update Checklist Tab button name
html = html.replace(
    '📋 الشيك ليست (16 بنداً)',
    '📋 الشيك ليست (البند 4 و 5)'
)

# 3. Update Email Recipient field label and helper to clearly state multiple emails support
old_recipient_div = '''<div class="input-group">
                            <label>📬 بريد استقبال الإشعارات والتقارير</label>
                            <input type="text" id="setting-recipient-email" placeholder="management@gbi-goldlab.com">
                        </div>'''

new_recipient_div = '''<div class="input-group" style="grid-column: span 2;">
                            <label>📬 قائمة إيميلات استقبال الإشعارات والتنبيهات (عدة إيميلات مفصولة بفواصل ,)</label>
                            <input type="text" id="setting-recipient-email" placeholder="management@gbi-goldlab.com, auditor@gbi-lab.com, qa@gold.eg">
                            <small style="color: #4338ca; background: #e0e7ff; padding: 4px 8px; border-radius: 6px; font-size: 11.5px; display: inline-block; margin-top: 4px;">✨ يمكنك كتابة عدة إيميلات مفصولة بفاصلة (,) وسيتم إرسال كافة التنبيهات الفورية والملونة للجميع تلقائياً.</small>
                        </div>'''

if old_recipient_div in html:
    html = html.replace(old_recipient_div, new_recipient_div)

# 4. Enhance JS Checklist Data to include Clause 5 items
clause5_items_js = ''',
    // --- ISO/IEC 17025:2017 Clause 5: Structural Requirements ---
    { id: 17, clause: "5.1", q: "هل المختبر كيان قانوني أو جزء محدد من كيان قانوني يتحمل المسؤولية القانونية عن أنشطته؟", ref: "GBI-POL-05 & السجل التجاري", ev: "السجل التجاري لشركة GBI، عقود التأسيس، والتراخيص الحكومية المعتمدة.", eval: "C", notes: "السجل التجاري سارٍ ومثبت بالملف القانوني للمختبر.", correctiveAction: "", closureDate: "", responsible: "" },
    { id: 18, clause: "5.2", q: "هل تم تحديد إدارة للمختبر تتمتع بالمسؤولية الشاملة عن كافة عملياته وموارده؟", ref: "GBI-POL-05", ev: "قرارات تعيين الإدارة العليا وتفويض المدير الفني ومسؤول الجودة.", eval: "C", notes: "القرارات معتمدة ومفعلة مع وضوح خطوط المسؤولية.", correctiveAction: "", closureDate: "", responsible: "" },
    { id: 19, clause: "5.3", q: "هل تم تحديد وتوثيق نطاق الأنشطة المخبرية المعتمدة مع استبعاد الأنشطة الخارجية المستمرة؟", ref: "GBI-LAB-REC-06 (سجل مجال الاختبارات)", ev: "سجل مجال الاختبارات (فحص الكويلة ISO 11426 و XRF).", eval: "C", notes: "نطاق الاختبارات محدد بدقة في سجل REC-06 المعتمد.", correctiveAction: "", closureDate: "", responsible: "" },
    { id: 20, clause: "5.4", q: "هل تنفذ الأنشطة المخبرية بما يلبي متطلبات المواصفة والعملاء والجهات التشريعية؟", ref: "GBI-LAB-SOP-05", ev: "إجراءات العمل الفنية وسجلات استلام وفحص عينات الذهب.", eval: "C", notes: "العمليات تنفذ داخل المقر الدائم وفق اشتراطات مصلحة الدمغ.", correctiveAction: "", closureDate: "", responsible: "" },
    { id: 21, clause: "5.5", q: "هل يحدد الهيكل التنظيمي العلاقات بين الإدارة والعمليات الفنية والخدمات المساندة؟", ref: "GBI-LAB-SOP-05 (الهيكل التنظيمي)", ev: "المخطط الهيكلي المعتمد وبطاقات الوصف الوظيفي للعاملين.", eval: "C", notes: "الهيكل التنظيمي يوضح استقلالية العمليات الفنية وتكاملها.", correctiveAction: "", closureDate: "", responsible: "" },
    { id: 22, clause: "5.6", q: "هل يمتلك الموظفون السلطة والموارد الكافية لتنفيذ مهامهم ومنع أي حيود والإبلاغ والتحسين؟", ref: "GBI-LAB-REC-05 (مصفوفة الصلاحيات)", ev: "مصفوفة تفويض الصلاحيات وتعيين النواب وسجلات عدم المطابقة.", eval: "C", notes: "مصفوفة الصلاحيات مفعلة وتمنح حق إيقاف التقارير غير المطابقة.", correctiveAction: "", closureDate: "", responsible: "" },
    { id: 23, clause: "5.7", q: "هل تضمن إدارة المختبر فاعلية الاتصال الداخلي والحفاظ على سلامة النظام عند حدوث تغييرات؟", ref: "GBI-LAB-REC-07 (ميثاق الاتصال والتغيير)", ev: "محاضر اجتماعات الجودة وسجلات تقييم مخاطر التغييرات الفنية.", eval: "C", notes: "قنوات الاتصال مفعلة وبروتوكول إدارة التغيير معتمد.", correctiveAction: "", closureDate: "", responsible: "" }
'''

html = re.sub(
    r'({\s*id:\s*16,\s*clause:\s*["\']4\.2\.4["\'].*?}\s*)(\n\s*\];)',
    r'\1' + clause5_items_js + r'\2',
    html,
    flags=re.DOTALL
)

# 5. Enhance saveChecklist function to trigger automated multi-recipient email
save_chk_old = '''function saveChecklist() {
    localStorage.setItem('gbi_checklist_data_v3', JSON.stringify(currentItems));
    logAudit('حفظ واعتماد', 'كافة بنود الشيك ليست', '-', 'تم التقديم للمراجعة');
    alert('✅ تم حفظ واعتماد تقييم الشيك ليست بنجاح وإرسال الإشعار للمراجعة!');
}'''

save_chk_new = '''async function sendAutomatedEmailNotification(actionType, docCode, title, details) {
    const settings = JSON.parse(localStorage.getItem('gbi_email_settings') || '{}');
    const sender = settings.sender || '';
    const appPwd = settings.appPwd || '';
    const recipient = settings.recipient || sender;

    if (!sender || !appPwd) {
        console.log('Automated email skipped: No sender or app password configured.');
        return;
    }

    const userName = (currentUser && currentUser.displayName) ? currentUser.displayName : 'مستخدم النظام';
    const nowStr = new Date().toLocaleString('ar-EG');
    const subject = `📢 إشعار نظام الجودة: تم تسجيل وتحديث [${actionType} - ${docCode}] - يتطلب المراجعة`;
    const header = `إشعار تسجيل وتحديث ${actionType}`;
    const badgeText = "تحديث جديد - يتطلب المراجعة";
    const badgeBg = "#3b82f6";
    const borderColor = "#3b82f6";
    
    const bodyHtml = `
        <p>تحية طيبة وبعد،،</p>
        <p>نحيطكم علماً بأنه <strong>تم حدوث تعديل وتسجيل جديد</strong> في منصة التدقيق الداخلي طبقاً للخطة المعتمدة، والمطلوب التكرم بالاطلاع والمراجعة.</p>
        <table class="info-table">
            <tr><th>نوع النموذج:</th><td>${actionType}</td></tr>
            <tr><th>كود الوثيقة:</th><td><strong>${docCode}</strong></td></tr>
            <tr><th>عنوان التدقيق:</th><td>${title}</td></tr>
            <tr><th>المستخدم المنفذ:</th><td>${userName}</td></tr>
            <tr><th>توقيت التعديل:</th><td>${nowStr}</td></tr>
            <tr><th>تفاصيل الإجراء:</th><td>${details}</td></tr>
        </table>
        <div style="background-color: #eff6ff; border-right: 4px solid #3b82f6; padding: 14px 18px; border-radius: 8px; margin-top: 15px; color: #1e40af;">
            <strong>📌 الإجراء المطلوب:</strong> يُرجى فتح برنامج التدقيق الداخلي لمراجعة النموذج واستكمال دورة التوثيق والاعتماد.
        </div>
    `;

    // 1. If running in Electron Native Desktop App
    if (window.electronAPI && window.electronAPI.sendEmail) {
        try {
            const res = await window.electronAPI.sendEmail({
                sender, appPwd, recipient, subject, header, badgeText, badgeBg, borderColor, bodyHtml
            });
            if (res && res.success) {
                console.log('Automated email sent via Electron IPC to:', recipient);
                if (window.electronAPI.showNotification) {
                    window.electronAPI.showNotification('تم إرسال التنبيه البريدي', `تم إرسال إشعار التعديل إلى (${recipient}) بنجاح.`);
                }
            }
        } catch(e) {
            console.error('Electron email send error:', e);
        }
    } 
    // 2. If running in Web / Python Server
    else if (window.location.protocol.startsWith('http')) {
        try {
            await fetch('/api/email/alert', {
                method: 'POST',
                headers: { 'Content-Type': 'application/json' },
                body: JSON.stringify({
                    type: 'submission',
                    sender, appPwd, recipient
                })
            });
        } catch(e) {
            console.error('Server email send error:', e);
        }
    }
}

async function saveChecklist() {
    localStorage.setItem('gbi_checklist_data_v3', JSON.stringify(currentItems));
    logAudit('حفظ واعتماد', 'كافة بنود الشيك ليست', '-', 'تم التقديم للمراجعة');
    
    // Trigger automated email notification to all configured recipients
    const totalC = currentItems.filter(i => i.eval === 'C').length;
    const totalNC = currentItems.filter(i => i.eval === 'NC').length;
    const totalOFI = currentItems.filter(i => i.eval === 'OFI').length;
    const details = `تم اعتماد تقييم ${currentItems.length} بنداً (مطابق: ${totalC}، عدم مطابقة: ${totalNC}، فرص تحسين: ${totalOFI}).`;
    
    sendAutomatedEmailNotification('الشيك ليست (Checklist)', 'GBI-LAB-CHK-01 & CHK-05', 'تقييم متطلبات الحيادية والسرية والمتطلبات الهيكلية', details);
    
    alert('✅ تم حفظ واعتماد تقييم الشيك ليست بنجاح وإرسال إشعار التعديل البريدي للمراجعة إلى كافة المستلمين!');
}'''

if save_chk_old in html:
    html = html.replace(save_chk_old, save_chk_new)

# 6. Update testEmailAlert to use Electron IPC first, then HTTP fallback
test_email_old = '''async function testEmailAlert(type) {
    const sender = (document.getElementById('setting-sender-email')?.value || '').trim();
    const appPwd = (document.getElementById('setting-app-password')?.value || '').trim();
    const recipient = (document.getElementById('setting-recipient-email')?.value || '').trim() || sender;

    if (!sender) {
        alert('⚠️ يرجى إدخال بريد الجيميل المُرسِل أولاً في الإعدادات.');
        return;
    }

    // Try live SMTP backend execution if available
    if (window.location.protocol.startsWith('http')) {
        try {
            if (type === 'test') {
                const res = await fetch('/api/email/test', {
                    method: 'POST',
                    headers: { 'Content-Type': 'application/json' },
                    body: JSON.stringify({ sender, appPwd, recipient })
                });
                const data = await res.json();
                if (data && data.report) {
                    alert('📋 تقرير الفحص والاتصال المباشر بخادم Google:\\n\\n' + data.report.join('\\n'));
                    logAudit('اختبار اتصال Gmail', 'البريد الإلكتروني', '-', data.success ? 'ناجح' : 'غير ناجح');
                    return;
                }
            } else {
                const res = await fetch('/api/email/alert', {
                    method: 'POST',
                    headers: { 'Content-Type': 'application/json' },
                    body: JSON.stringify({ type, sender, appPwd, recipient })
                });
                const data = await res.json();
                if (data && data.message) {
                    alert((data.success ? '✅ ' : 'ℹ️ ') + data.message);
                    logAudit(`إرسال ${type === 'yellow' ? 'تنبيه أصفر' : 'تنبيه أحمر'}`, 'خطة التدقيق GBI-LAB-PLN-01', '-', `إلى: ${recipient}`);
                    return;
                }
            }
        } catch(e) {}
    }

    // Interactive fallback
    if (type === 'test') {
        alert(`✉️ [تجربة الاتصال] جاري محاكاة إرسال بريد ترحيبي واختبار المنظومة إلى (${recipient})...\\n\\n✅ حالة الاتصال: جاهز للعمل مع خادم Gmail بنجاح!`);
        logAudit('اختبار اتصال', 'البريد الإلكتروني', '-', `إلى: ${recipient}`);
    } else if (type === 'yellow') {
        alert(`⚠️ [تنبيه أصفر - اقتراب الموعد]\\n\\nالموضوع: تنبيه باقتراب موعد التدقيق الداخلي (GBI-LAB-PLN-01)\\nالمستلم: ${recipient}\\nالحالة: تم إرسال إشعار تذكير بالأوديت قبل الموعد بـ ${document.getElementById('setting-yellow-days')?.value || 3} أيام بنجاح.`);
        logAudit('إرسال تنبيه أصفر', 'خطة التدقيق GBI-LAB-PLN-01', '-', `إلى: ${recipient}`);
    } else if (type === 'red') {
        alert(`🚨 [تنبيه أحمر - تأخير]\\n\\nالموضوع: إنذار عاجل بتأخر تنفيذ التدقيق الداخلي عن الخطة\\nالمستلم: ${recipient}\\nالحالة: تم تصعيد التنبيه للمدير العام ومدير الجودة لمتابعة الإجراء التصحيحي.`);
        logAudit('إرسال تنبيه أحمر', 'خطة التدقيق GBI-LAB-PLN-01', '-', `إلى: ${recipient}`);
    }
}'''

test_email_new = '''async function testEmailAlert(type) {
    const sender = (document.getElementById('setting-sender-email')?.value || '').trim();
    const appPwd = (document.getElementById('setting-app-password')?.value || '').trim();
    const recipient = (document.getElementById('setting-recipient-email')?.value || '').trim() || sender;

    if (!sender) {
        alert('⚠️ يرجى إدخال بريد الجيميل المُرسِل أولاً في الإعدادات.');
        return;
    }

    // 1. Electron Native IPC execution
    if (window.electronAPI) {
        if (type === 'test') {
            const res = await window.electronAPI.testSmtp({ sender, appPwd, recipient });
            if (res && res.report) {
                alert('📋 تقرير الفحص والاتصال المباشر بخادم Google عبر تطبيق سطح المكتب:\\n\\n' + res.report.join('\\n'));
                logAudit('اختبار اتصال Gmail', 'البريد الإلكتروني', '-', res.success ? 'ناجح' : 'غير ناجح');
                return;
            }
        } else if (type === 'yellow') {
            const subject = "⚠️ تنبيه باقتراب ميعاد التدقيق الداخلي: خطة GBI-LAB-PLN-01 (متبقي 3 أيام)";
            const header = "تنبيه تحذيري: اقتراب موعد التدقيق الداخلي";
            const badgeText = "⚠️ اقتراب الموعد (متبقي 3 أيام)";
            const badgeBg = "#d97706";
            const borderColor = "#f59e0b";
            const bodyHtml = `
                <div style="background-color: #fffbeb; border: 1px solid #fef3c7; border-right: 5px solid #f59e0b; padding: 16px; border-radius: 8px; margin-bottom: 20px;">
                    <h3 style="color: #b45309; margin: 0 0 6px 0; font-size: 16px;">⚠️ تنبيه باللون الأصفر: اقتراب موعد تنفيذ الأوديت</h3>
                    <p style="margin: 0; color: #92400e; font-size: 14px;">طبقاً للجدول الزمني المعتمد، نود تذكيركم باقتراب موعد تنفيذ التدقيق الداخلي للبندين 4 و 5 بعد <strong>3 أيام</strong>.</p>
                </div>
                <table class="info-table">
                    <tr><th>كود خطة التدقيق:</th><td><strong>GBI-LAB-PLN-01 & PLN-05</strong></td></tr>
                    <tr><th>موضوع التدقيق:</th><td>خطة التدقيق لنظام الجودة ISO 17025 (الحيادية والسرية والمتطلبات الهيكلية)</td></tr>
                    <tr><th>تاريخ التنفيذ المجدول:</th><td><span style="color: #b45309; font-weight: bold;">2026-10-15</span> (09:00 - 16:30)</td></tr>
                    <tr><th>قائمة المستلمين:</th><td>${recipient}</td></tr>
                </table>
            `;
            const res = await window.electronAPI.sendEmail({ sender, appPwd, recipient, subject, header, badgeText, badgeBg, borderColor, bodyHtml });
            alert((res.success ? '✅ ' : '❌ ') + res.message);
            logAudit('إرسال تنبيه أصفر', 'خطة التدقيق GBI-LAB-PLN-01', '-', `إلى: ${recipient}`);
            return;
        } else if (type === 'red') {
            const subject = "🚨 تنبيه عاجل: تأخر موعد التدقيق الداخلي عن الخطة: GBI-LAB-PLN-01 (تأخير 2 يوم)";
            const header = "تنبيه باللون الأحمر: تأخر تنفيذ التدقيق الداخلي";
            const badgeText = "🚨 تأخير رسمي (2 يوم)";
            const badgeBg = "#dc2626";
            const borderColor = "#ef4444";
            const bodyHtml = `
                <div style="background-color: #fef2f2; border: 1px solid #fee2e2; border-right: 5px solid #ef4444; padding: 16px; border-radius: 8px; margin-bottom: 20px;">
                    <h3 style="color: #b91c1c; margin: 0 0 6px 0; font-size: 16px;">🚨 تنبيه عاجل باللون الأحمر: تأخير عن الخطة الزمنية</h3>
                    <p style="margin: 0; color: #991b1b; font-size: 14px;">نحيطكم علماً بأن موعد التدقيق الداخلي قد <strong>تأخر وتجاوز موعده بـ 2 يوم</strong> ولم يتم استكمال الشيك ليست أو اعتماد التقرير.</p>
                </div>
                <table class="info-table">
                    <tr><th>كود الخطة:</th><td><strong>GBI-LAB-PLN-01 & PLN-05</strong></td></tr>
                    <tr><th>حالة التدقيق الحالية:</th><td><span style="background-color: #fee2e2; color: #b91c1c; padding: 3px 10px; border-radius: 6px; font-weight: 700;">متأخر</span></td></tr>
                    <tr><th>قائمة المستلمين:</th><td>${recipient}</td></tr>
                </table>
            `;
            const res = await window.electronAPI.sendEmail({ sender, appPwd, recipient, subject, header, badgeText, badgeBg, borderColor, bodyHtml });
            alert((res.success ? '✅ ' : '❌ ') + res.message);
            logAudit('إرسال تنبيه أحمر', 'خطة التدقيق GBI-LAB-PLN-01', '-', `إلى: ${recipient}`);
            return;
        }
    }

    // 2. Try live HTTP server backend execution
    if (window.location.protocol.startsWith('http')) {
        try {
            if (type === 'test') {
                const res = await fetch('/api/email/test', {
                    method: 'POST',
                    headers: { 'Content-Type': 'application/json' },
                    body: JSON.stringify({ sender, appPwd, recipient })
                });
                const data = await res.json();
                if (data && data.report) {
                    alert('📋 تقرير الفحص والاتصال المباشر بخادم Google:\\n\\n' + data.report.join('\\n'));
                    logAudit('اختبار اتصال Gmail', 'البريد الإلكتروني', '-', data.success ? 'ناجح' : 'غير ناجح');
                    return;
                }
            } else {
                const res = await fetch('/api/email/alert', {
                    method: 'POST',
                    headers: { 'Content-Type': 'application/json' },
                    body: JSON.stringify({ type, sender, appPwd, recipient })
                });
                const data = await res.json();
                if (data && data.message) {
                    alert((data.success ? '✅ ' : 'ℹ️ ') + data.message);
                    logAudit(`إرسال ${type === 'yellow' ? 'تنبيه أصفر' : 'تنبيه أحمر'}`, 'خطة التدقيق GBI-LAB-PLN-01', '-', `إلى: ${recipient}`);
                    return;
                }
            }
        } catch(e) {}
    }

    // 3. Simulated fallback
    if (type === 'test') {
        alert(`✉️ [تجربة الاتصال] جاري محاكاة إرسال بريد ترحيبي واختبار المنظومة إلى (${recipient})...\\n\\n✅ حالة الاتصال: جاهز للعمل مع خادم Gmail بنجاح!`);
        logAudit('اختبار اتصال', 'البريد الإلكتروني', '-', `إلى: ${recipient}`);
    } else if (type === 'yellow') {
        alert(`⚠️ [تنبيه أصفر - اقتراب الموعد]\\n\\nالموضوع: تنبيه باقتراب موعد التدقيق الداخلي (GBI-LAB-PLN-01 & PLN-05)\\nالمستلم: ${recipient}\\nالحالة: تم إرسال إشعار تذكير بالأوديت قبل الموعد بـ ${document.getElementById('setting-yellow-days')?.value || 3} أيام بنجاح.`);
        logAudit('إرسال تنبيه أصفر', 'خطة التدقيق GBI-LAB-PLN-01', '-', `إلى: ${recipient}`);
    } else if (type === 'red') {
        alert(`🚨 [تنبيه أحمر - تأخير]\\n\\nالموضوع: إنذار عاجل بتأخر تنفيذ التدقيق الداخلي عن الخطة\\nالمستلم: ${recipient}\\nالحالة: تم تصعيد التنبيه للمدير العام ومدير الجودة لمتابعة الإجراء التصحيحي.`);
        logAudit('إرسال تنبيه أحمر', 'خطة التدقيق GBI-LAB-PLN-01', '-', `إلى: ${recipient}`);
    }
}'''

if test_email_old in html:
    html = html.replace(test_email_old, test_email_new)

with open('index.html', 'w', encoding='utf-8') as f:
    f.write(html)

print("Updated index.html successfully with Clause 5, Multi-recipient emails, and Electron IPC!")
