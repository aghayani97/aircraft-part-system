<!-- واتساپ - اضافه شده توسط دستیار -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
<style>
    /* واتساپ Floating Button */
    .whatsapp-float {
        position: fixed;
        width: 60px;
        height: 60px;
        bottom: 25px;
        right: 25px;
        background-color: #25d366;
        color: white;
        border-radius: 50%;
        text-align: center;
        font-size: 32px;
        box-shadow: 0 4px 15px rgba(37, 211, 102, 0.5);
        z-index: 10000;
        display: flex;
        align-items: center;
        justify-content: center;
        text-decoration: none;
        transition: all 0.3s ease;
        animation: whatsapp-pulse 2s infinite;
    }
    
    .whatsapp-float:hover {
        background-color: #128C7E;
        transform: scale(1.1);
        box-shadow: 0 6px 25px rgba(37, 211, 102, 0.7);
    }
    
    @keyframes whatsapp-pulse {
        0% { box-shadow: 0 0 0 0 rgba(37, 211, 102, 0.7); }
        70% { box-shadow: 0 0 0 15px rgba(37, 211, 102, 0); }
        100% { box-shadow: 0 0 0 0 rgba(37, 211, 102, 0); }
    }
    
    /* واتساپ Section در صفحه */
    .whatsapp-section {
        background: linear-gradient(135deg, #f0fff4 0%, #e6fffa 100%);
        border: 2px solid #25d366;
        border-radius: 15px;
        padding: 25px;
        margin: 40px 0;
        text-align: center;
        position: relative;
        overflow: hidden;
    }
    
    .whatsapp-section::before {
        content: "";
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        height: 4px;
        background: linear-gradient(90deg, #25d366, #128C7E);
    }
    
    .whatsapp-title {
        color: #075E54;
        margin-bottom: 15px;
        font-size: 22px;
        display: flex;
        align-items: center;
        justify-content: center;
        gap: 10px;
    }
    
    .whatsapp-btn {
        display: inline-block;
        background: linear-gradient(135deg, #25d366, #128C7E);
        color: white;
        padding: 14px 28px;
        border-radius: 50px;
        text-decoration: none;
        font-weight: bold;
        margin: 10px 5px;
        transition: all 0.3s;
        border: none;
        cursor: pointer;
        font-size: 16px;
        box-shadow: 0 4px 12px rgba(37, 211, 102, 0.3);
    }
    
    .whatsapp-btn:hover {
        transform: translateY(-3px);
        box-shadow: 0 8px 20px rgba(37, 211, 102, 0.5);
        background: linear-gradient(135deg, #128C7E, #25d366);
    }
    
    .whatsapp-options {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        gap: 12px;
        margin: 20px 0;
    }
    
    .whatsapp-option {
        background: white;
        color: #075E54;
        border: 2px solid #c6f6d5;
        padding: 12px 20px;
        border-radius: 8px;
        text-decoration: none;
        transition: all 0.3s;
        min-width: 160px;
        text-align: center;
        font-size: 14px;
    }
    
    .whatsapp-option:hover {
        background: #25d366;
        color: white;
        border-color: #25d366;
        transform: translateY(-2px);
    }
    
    .whatsapp-info {
        background: #f8f9fa;
        padding: 15px;
        border-radius: 10px;
        margin-top: 20px;
        font-size: 15px;
        color: #555;
    }
    
    /* ریسپانسیو برای موبایل */
    @media (max-width: 768px) {
        .whatsapp-float {
            width: 55px;
            height: 55px;
            bottom: 20px;
            right: 20px;
            font-size: 28px;
        }
        
        .whatsapp-section {
            padding: 20px 15px;
            margin: 30px 0;
        }
        
        .whatsapp-options {
            flex-direction: column;
            align-items: center;
        }
        
        .whatsapp-option {
            width: 100%;
            max-width: 300px;
        }
    }
</style>
