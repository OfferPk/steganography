How It Works
This tool uses steganography to hide secret messages within images. The message is embedded in the least significant bits (LSB) of the image's pixel data, making it invisible to the naked eye. The tool also supports symmetric encryption (XOR, AES) to protect the hidden data.

Key Features
LSB Embedding: Modifies the least significant bits of pixel values to store hidden data.
Channel Selection: Choose which color channel (RGB) to use for embedding.
Encryption Options: Simple XOR for basic protection or AES for stronger encryption.
Capacity Display: Shows maximum text length based on image size and settings.
Step-by-Step Guide
Upload an Image:
Click the '📁' area or drag & drop a PNG image.
Supported formats: PNG (lossless, best for steganography), JPEG (may distort data).
Configure Settings:
LSB Mode: Choose 1-bit (more data), 2-bit (balance), or 4-bit (better quality).
Color Channel: Select 'All channels' or a specific channel (R/G/B).
Encryption:
'None': No encryption (default).
'Simple XOR': Basic encryption with a password.
'AES': Strong encryption (requires CryptoJS library).
Enter Secret Message:
Type your text in the 'Enter your secret message here...' box.
The placeholder shows the maximum character limit based on your settings.
Hide Text:
Click '🔒 Hide Text' to embed the message in the image.
A progress bar shows the embedding process.
A download link appears when complete ('secret_[filename].png').
Extract Text:
Upload the steganographed image.
Click '🔓 Extract Text' to retrieve the hidden message.
If encrypted, enter the password for decryption.
Reset:
Click '🔄 Reset' to restore the original image and clear fields.
Best Practices
Use PNG images for optimal results (JPEG may corrupt data).
Keep messages under the capacity limit (displayed in the text box).
For encryption, use strong passwords and share them securely.
Test with small messages first to verify functionality.
Limitations
Text must be ASCII-compatible (UTF-8 support limited).
Large images may take longer to process.
Encryption algorithms (AES) require external libraries.
Hidden data is not secure against advanced analysis.
code area 
```html
<div class="card">
    <h2>How It Works</h2>
    <p>This tool uses <strong>steganography</strong> to hide secret messages within images. The message is embedded in the <strong>least significant bits (LSB)</strong> of the image's pixel data, making it invisible to the naked eye. The tool also supports <strong>symmetric encryption</strong> (XOR, AES) to protect the hidden data.</p>
    
    <h3>Key Features</h3>
    <ul>
        <li><strong>LSB Embedding:</strong> Modifies the least significant bits of pixel values to store hidden data.</li>
        <li><strong>Channel Selection:</strong> Choose which color channel (RGB) to use for embedding.</li>
        <li><strong>Encryption Options:</strong> Simple XOR for basic protection or AES for stronger encryption.</li>
        <li><strong>Capacity Display:</strong> Shows maximum text length based on image size and settings.</li>
    </ul>

    <h3>Step-by-Step Guide</h3>
    <ol>
        <li><strong>Upload an Image:</strong>
            <ul>
                <li>Click the "📁" area or drag & drop a PNG image.</li>
                <li>Supported formats: PNG (lossless, best for steganography), JPEG (may distort data).</li>
            </ul>
        </li>
        <li><strong>Configure Settings:</strong>
            <ul>
                <li><strong>LSB Mode:</strong> Choose 1-bit (more data), 2-bit (balance), or 4-bit (better quality).</li>
                <li><strong>Color Channel:</strong> Select "All channels" or a specific channel (R/G/B).</li>
                <li><strong>Encryption:</strong> 
                    <ul>
                        <li>"None": No encryption (default).</li>
                        <li>"Simple XOR": Basic encryption with a password.</li>
                        <li>"AES": Strong encryption (requires CryptoJS library).</li>
                    </ul>
                </li>
            </ul>
        </li>
        <li><strong>Enter Secret Message:</strong>
            <ul>
                <li>Type your text in the "Enter your secret message here..." box.</li>
                <li>The placeholder shows the maximum character limit based on your settings.</li>
            </ul>
        </li>
        <li><strong>Hide Text:</strong>
            <ul>
                <li>Click "🔒 Hide Text" to embed the message in the image.</li>
                <li>A progress bar shows the embedding process.</li>
                <li>A download link appears when complete ("secret_[filename].png").</li>
            </ul>
        </li>
        <li><strong>Extract Text:</strong>
            <ul>
                <li>Upload the steganographed image.</li>
                <li>Click "🔓 Extract Text" to retrieve the hidden message.</li>
                <li>If encrypted, enter the password for decryption.</li>
            </ul>
        </li>
        <li><strong>Reset:</strong>
            <ul>
                <li>Click "🔄 Reset" to restore the original image and clear fields.</li>
            </ul>
        </li>
    </ol>

    <h3>Best Practices</h3>
    <ul>
        <li>Use <strong>PNG images</strong> for optimal results (JPEG may corrupt data).</li>
        <li>Keep messages <strong>under the capacity limit</strong> (displayed in the text box).</li>
        <li>For encryption, use <strong>strong passwords</strong> and share them securely.</li>
        <li>Test with small messages first to verify functionality.</li>
    </ul>

    <h3>Limitations</h3>
    <ul>
        <li>Text must be <strong>ASCII-compatible</strong> (UTF-8 support limited).</li>
        <li>Large images may take longer to process.</li>
        <li>Encryption algorithms (AES) require external libraries.</li>
        <li>Hidden data is <strong>not secure against advanced analysis</strong>.</li>
    </ul>
</div>
```
